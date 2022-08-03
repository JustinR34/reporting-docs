---
title: demo
page_title: demo
description: demo
slug: telerikreporting/demo
tags: demo
published: True
position: 2
---

# How to Add Telerik Reporting REST Web API to Web Application

In this case the Web API will be hosted on top of the classic ASP.NET hosting infrastructure, supported by the IIS (Internet Information Services) server. The REST service setup can be done either by using the Telerik Reporting REST Service project template or manually, as explained below. 

## Using the REST Service Project Template

In Visual Studio open the __Add New Project__ dialog and select *Telerik Reporting REST Service* project template, which appears when selecting __Reporting__ category from the left pane. This will add a new project in your solution that contains all the necessary files and packages to host the Telerik Reporting REST service instance. 

The project has a preconfigured implementation of reports controller that uses the *"~\Reports"* path for its report source resolver. This directory is not automatically created and needs to be created, or the path to be modified accordingly prior to running the project. 

## Manually configuring Telerik.Reporting REST Service on IIS

###To host and configure the Telerik.Reporting REST Service on IIS follow the steps below:

1. In Visual Studio, create the hosting project. That might be one of the following project templates: ASP.NET Empty Web Application, ASP.NET Web Forms Application, ASP.NET MVC Web Application. 

1. Make sure that the project has the following assembly references: 

   + Newtonsoft.Json.dll 

   + System.Web.Http.dll 

   + System.Web.Http.WebHost.dll 

   + System.Net.Http.dll 

   + System.Net.Http.Formatting.dll 

1. Invoke 0 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

	```C#
	protected void Application_Start()
	{
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	}
	```
	```VB
	Sub Application_Start()
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	End Sub
	```


1. Invoke 1 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

	```C#
	protected void Application_Start()
	{
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	}
	```
	
	```VB
	Sub Application_Start()
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	End Sub
	```


1. Invoke 2 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

	```C#
		protected void Application_Start()
		{
			ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
			ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
			ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		}
	```
	```VB
		Sub Application_Start()
			ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
			ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
			ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		End Sub
	```


1. Invoke 3 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

	```C#
		protected void Application_Start()
		{
			ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
			ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
			ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		}
	```
	
	```VB
		Sub Application_Start()
			ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
			ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
			ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		End Sub
	```


1. Invoke 4 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

	```C#
protected void Application_Start()
	{
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	}
```
	```VB
Sub Application_Start()
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	End Sub
```


1. Invoke 5 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

	```C#
protected void Application_Start()
	{
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	}
```

	```VB
Sub Application_Start()
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	End Sub
```


1. Invoke 6 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

	```C#
protected void Application_Start()
{
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
}
```
	```VB
Sub Application_Start()
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
End Sub
```


1. Invoke 7 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

	```C#
protected void Application_Start()
{
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
}
```

	```VB
Sub Application_Start()
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
End Sub
```


1. Invoke 8 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

	```C#
	protected void Application_Start()
	{
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	}
```
	```VB
	Sub Application_Start()
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	End Sub
```


1. Invoke 9 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

	```C#
	protected void Application_Start()
	{
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	}
```

	```VB
	Sub Application_Start()
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	End Sub
```


1. Invoke 10 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

```C#
protected void Application_Start()
{
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
}
```
```VB
Sub Application_Start()
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
End Sub
```


1. Invoke 11 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

```C#
protected void Application_Start()
{
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
}
```

```VB
Sub Application_Start()
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
End Sub
```


1. Invoke 12 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

	```C#
	protected void Application_Start()
	{
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	}

	```VB
	Sub Application_Start()
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	End Sub
	```


1. Invoke 13 RegisterRoutes `Global.Application_Start (Global.asax)` method: 

	```C#
	protected void Application_Start()
	{
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration);
	}
	
	
	```VB
	Sub Application_Start()
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
		ReportsControllerConfiguration.RegisterRoutes(GlobalConfiguration.Configuration)
	End Sub
	```

