---
title: "Get installed app in chat"
description: "Get installed app in a chat."
author: "nkramer"
localization_priority: Priority
ms.prod: "microsoft-teams"
doc_type: apiPageType
---

# Get installed app in chat

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get [app installation](../resources/teamsappinstallation.md) installed in a [chat](../resources/chat.md).

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All

## HTTP request

<!-- { 
"blockType": "ignored" 
} -->

```http
GET /chats/{chatId}/installedApps/{appInstallationId}
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Response

If successful, this method returns a `200 OK` and a [teamsApp](../resources/teamsapp.md) object in the body.

## Example: Get an app installed in the specified chat

### Request

<!-- {
  "blockType": "request",
  "name": "get_installedApp"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{chatid}/installedApps/{appInstallationId}

```

### Response

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->

```http
HTTP/1.1 200 OK

Content-Type: application/json
{
   "value": {
      "@odata.type":"#microsoft.graph.chat",
      "id":"e8127558-91ad-4595-8703-6e1ed3f04bfe",
      "topic":"Get installed app in chat",
      "createdDateTime":"2020-10-27 23:52:29",
      "lastEditedDateTime":"2020-10-27 23:52:29"
   }
}
`