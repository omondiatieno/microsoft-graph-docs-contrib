---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

// Dependencies
using Microsoft.Graph.Beta.Models;

var requestBody = new Subscription
{
	ChangeType = "created",
	NotificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient",
	Resource = "me/mailfolders('Drafts')/messages?$select=Subject,bodyPreview&$filter=hasAttachments eq true AND importance eq 'High'",
	ExpirationDateTime = DateTimeOffset.Parse("2022-01-01T21:42:18.2257768+00:00"),
	ClientState = "secretClientValue",
	IncludeResourceData = true,
	EncryptionCertificate = "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
	EncryptionCertificateId = "testCertificateId",
};

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=csharp
var result = await graphClient.Subscriptions.PostAsync(requestBody);


```