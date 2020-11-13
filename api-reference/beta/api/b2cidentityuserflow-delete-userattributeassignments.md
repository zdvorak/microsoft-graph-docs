---
title: "Delete userAttributeAssignments from b2cIdentityUserFlow"
description: "Delete an identityUserFlowAttributeAssignment object from a b2cIdentityUserFlow."
author: "jkdouglas"
localization_priority: Normal
ms.prod: "microsoft-identity-platform"
doc_type: apiPageType
---

# Delete userAttributeAssignments from b2cIdentityUserFlow

Namespace: microsoft.graph

Delete an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|External Identity User Flow Administrator, Global Administrator|
|Delegated (personal Microsoft account)|Not supported|
|Application|External Identity User Flow Administrator, Global Administrator|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "delete_userattributeassignments_from_b2cidentityuserflow"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```

### Response

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```