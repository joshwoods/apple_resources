

- App Store Connect API
-  Read queue information 

Web Service Endpoint

# Read queue information

Get information about a specific queue and its related objects.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the queue.

## Query Parameters

`fields[gameCenterMatchmakingQueues]`

`[string]`

The fields of the queue to include in the response.

Possible Values: `referenceName, classicMatchmakingBundleIds, ruleSet, experimentRuleSet`

`include`

`[string]`

The type of rule set to include in the response.

Possible Values: `ruleSet, experimentRuleSet`

## Response Codes

` 200 ``OK`

GameCenterMatchmakingQueueResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## See Also

### Reading queue information

List all queues

Get information about all queues.

