---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

// Dependencies
using Microsoft.Graph.Models;

var requestBody = new ExtensionProperty
{
	Name = "jobGroup",
	DataType = "String",
	TargetObjects = new List<string>
	{
		"User",
	},
};

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=csharp
var result = await graphClient.Applications["{application-id}"].ExtensionProperties.PostAsync(requestBody);


```