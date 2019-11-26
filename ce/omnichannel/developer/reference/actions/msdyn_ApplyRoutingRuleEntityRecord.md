---
title: "msdyn_ApplyRoutingRuleEntityRecord Action Reference (Developer Guide for Dynamics 365 Customer Engagement)| MicrosoftDocs"
description: "Reference information about the msdyn_ApplyRoutingRuleEntityRecord Action."
author: "susikka"
ms.author: "susikka"
manager: "shujoshi"
applies_to: 
  - "Dynamics 365 (online)"
ms.date: 10/03/2019
ms.service: 
  - crm-online
ms.topic: "reference"
---
# msdyn_ApplyRoutingRuleEntityRecord Action Reference

Applies the active routing rule to an entity.

**Owning Solution**: Microsoft.Dynamics.CRM.System

## Parameters

Parameters allow for data to be passed to the action.


| Name | Type | Nullable | Unicode | Description |
|------|------|------|------|------|
| Target | Microsoft.Dynamics.CRM.crmbaseentity | False | True | The entity to apply the routing rule to.|

## Return value

This action has no return value.

## Entities

This action will apply to entities which have Routing Rule set to active.

## Example

The example given below shows how you can create a Web API request to call `msdyn_ApplyRoutingRuleEntityRecord` action for `Incident` entity.

**Request**

```http
POST [Organization URI]/api/data/v9.1/msdyn_ApplyRoutingRuleEntityRecord
Accept: application/json
Content-Type: application/json; charset=utf-8
OData-MaxVersion: 4.0
OData-Version: 4.0

{
    "Target":"incidents(<incidentid>)"
}
```

**Response**

```http
HTTP 204 No Content
```

### See also

[Developer guide for Omnichannel for Customer Service](../../omnichannel-developer.md)