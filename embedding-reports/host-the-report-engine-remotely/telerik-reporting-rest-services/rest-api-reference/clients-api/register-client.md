---
title: Register Client
page_title: Register Client 
description: Register Client
slug: telerikreporting/using-reports-in-applications/host-the-report-engine-remotely/telerik-reporting-rest-services/rest-api-reference/clients-api/register-client
tags: register,client
published: True
position: 0
previous_url: /telerik-reporting-rest-api-register-client
---

# Register Client

## Request
    
	POST /api/reports/clients

## Response

| HTTP Status Code | Description |
| ------ | ------ |
|`200 OK`|Client registered successfully|

__Response Body__ 

The body contains the newly registered client’s identifier.         

## Sample

* Request 

		POST /api/reports/clients HTTP/1.1

* Response 

		HTTP/1.1 200 OK
		
		{"clientId":"a5f3"}
