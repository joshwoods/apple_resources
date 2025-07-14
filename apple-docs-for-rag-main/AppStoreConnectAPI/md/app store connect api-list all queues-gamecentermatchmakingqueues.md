

- App Store Connect API
-  List all queues 

Web Service Endpoint

# List all queues

Get information about all queues.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues
```

## Query Parameters

`fields[gameCenterMatchmakingQueues]`

`[string]`

The fields of the queues to include in the response.

Possible Values: `referenceName, classicMatchmakingBundleIds, ruleSet, experimentRuleSet`

`include`

`[string]`

The type of rule set to include in the response.

Possible Values: `ruleSet, experimentRuleSet`

`limit`

`integer`

The maximum number of queues to fetch.

Maximum: `200`

## Response Codes

` 200 ``OK`

GameCenterMatchmakingQueuesResponse

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

## See Also

### Reading queue information

Read queue information

Get information about a specific queue and its related objects.

