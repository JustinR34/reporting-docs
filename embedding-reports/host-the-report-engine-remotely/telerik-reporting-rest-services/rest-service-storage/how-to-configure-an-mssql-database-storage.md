---
title: How to Configure an MSSQL Database Storage
page_title: How to Configure an MSSQL Database Storage 
description: How to Configure an MSSQL Database Storage
slug: telerikreporting/using-reports-in-applications/host-the-report-engine-remotely/telerik-reporting-rest-services/rest-service-storage/how-to-configure-an-mssql-database-storage
tags: how,to,configure,an,mssql,database,storage
published: True
position: 1
previous_url: /telerik-reporting-rest-howto-use-mssql-storage
---

# How to Configure an MSSQL Database Storage

This article will explain how to configure an MSSQL database for report engine storage.

## How to configure an MSSQL database storage:

1. Ensure a database instance is available for report engine storage. This may be a dedicated database or a shared database for both app data and report engine storage. 

	1. Start the __Telerik Database Cache Configurator__ tool located in the *{Telerik Reporting installation folder}/Tools* folder. 

	1. In *Choose database usage* combo-box select the "Configure REST service storage database" option. 

	1. In *Choose target backend* combo-box select the "Microsoft SQL Server" option. 

	1. In *Specify connection string* text box enter the connection string that references the target database. You can also click the *Build* button and create the connection string using the *Connection properties* form. 

	1. Click on the *Create schema* button to start the database schema creation. 

	1. A message box should be displayed, confirming that the storage tables are successfully created. Use the connection string specified above when initializing an instance of [MsSqlServerStorage](/reporting/api/Telerik.Reporting.Cache.MsSqlServerStorage) in your application. 

	1. In case you want to cleanup the storage tables in an existing database, use the button *Clear cache data*. 

1. Configure your Telerik Reporting REST Service to use the database storage we just prepared. You may do this in the configuration file of the project as elaborated in the article [restReportService Element]({%slug telerikreporting/using-reports-in-applications/export-and-configure/configure-the-report-engine/restreportservice-element%}), or when instantiating the [ReportServiceConfiguration](/reporting/api/Telerik.Reporting.Services.ReportServiceConfiguration). Here are samples for both scenarios: 

	+ Through code when passing [ReportServiceConfiguration](/reporting/api/Telerik.Reporting.Services.ReportServiceConfiguration) instance to the REST Service. 

		The __ReportSourceResolver__ and __Storage__ configuration settings are required. See the [IReportServiceConfiguration](/reporting/api/Telerik.Reporting.Services.IReportServiceConfiguration) interface for more details. 

		{{source=CodeSnippets\MvcCS\Controllers\ReportsController.cs region=MSSqlReportsControllerImplementation}}
		{{source=CodeSnippets\MvcVB\Controllers\ReportsController.vb region=MSSqlReportsControllerImplementation}}


	+ Through a configuration file: 

		1. You need to pass a [ConfigSectionReportServiceConfiguration](/reporting/api/Telerik.Reporting.Services.ConfigSectionReportServiceConfiguration) instance to the REST Service: 

			{{source=CodeSnippets\MvcCS\Controllers\ReportsControllerConfigSection.cs region=ReportsControllerConfigSectionImplementation}}
			{{source=CodeSnippets\MvcVB\Controllers\ReportsControllerConfigSection.vb region=ReportsControllerConfigSectionImplementation}}


			The properties from the initialization block would override the values obtained from the configuration file. 

		1. Set the corresponding properties values in the REST Service configuration file: 

			+ XML-based configuration file: 

				````XML
<configuration>
				...
				  <Telerik.Reporting>
					<restReportService hostAppId="Application1" workerCount="4" reportSharingTimeout="10" clientSessionTimeout="10" exceptionsVerbosity="detailed">
					  <reportResolver provider="type" />
					  <storage provider="MSSQLServer">
						<parameters>
						  <parameter name="connectionString" value="Data Source=(local)\SQLEXPRESS;Initial Catalog=RestServiceStorage;Integrated Security=SSPI" />
						  <parameter name="commandTimeout" value="60" />
						</parameters>
					  </storage>
				   ...
					  </restReportService>
				   ...
				  </Telerik.Reporting>
				...
				</configuration>
````


			+ JSON-based configuration file: 

				````JSON
"telerikReporting": {
				  "restReportService": {
					"hostAppId": "Application1",
					"reportResolver": {
					  "provider": "type"
					},
					"storage": {
					  "provider": "MSSQLServer",
					  "parameters": [
						{
						  "name": "connectionString",
						  "value": "Data Source=(local)\SQLEXPRESS;Initial Catalog=RestServiceStorage;Integrated Security=SSPI"
						},
						{
						  "name": "commandTimeout",
						  "value": 60
						}
				   ]
					}
				  },
				...
				}
````


## See Also

* [Overview]({%slug telerikreporting/using-reports-in-applications/host-the-report-engine-remotely/telerik-reporting-rest-services/rest-service-storage/overview%})
