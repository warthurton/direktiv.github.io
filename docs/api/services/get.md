---
layout: default
title: Get
nav_order: 4
parent: Services
grand_parent: API
has_children: false
---

# Get Service

API on how to get a Service

## Get Service 

**URL**: `{{ _.address }}/functions/{{_.serviceName}}`

**Method**: `GET`

**Input**

Providing 'serviceName' as parameter depending on whether it is global or namespace specific determines the outcome. If I have a service called 'test' and want to reference it as a namespace variable the service name would be `ns-NAMESPACE-test`. Globally the service name would be `g-test` instead.

## Success Response

**Code**: `200 Ok`

## Error Response

**Code**: `400 Bad Request`

**Content**

```json
{
    "Code": 400,
    "Message": "An error relating to the request"
}
```