---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPermissionCollectionPage permissions = graphClient.sites("{sitesId}").permissions()
	.buildRequest()
	.get();

```