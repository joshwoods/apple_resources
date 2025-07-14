

- App Store Connect API
-  Get matchmaking rule errors 

Web Service Endpoint

# Get matchmaking rule errors

Get errors that occur for a specific matchmaking rule.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingRules/{id}/metrics/matchmakingRuleErrors
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the rule.

## Query Parameters

`filter[gameCenterMatchmakingQueue]`

`string`

The fields of the queues to include in the response.

`granularity`

`string`

 (Required) 

The level of information you want in the response, specified as a time interval for the data collection, using the ISO 8601 format for durations.

Possible Values: `P1D, PT1H, PT15M`

`groupBy`

`[string]`

Organizes the results by queue.

Value: `gameCenterMatchmakingQueue`

`limit`

`integer`

The maximum number of results to include.

Maximum: `200`

`sort`

`[string]`

Sort results by the decreasing or increasing number of players that Game Center finds.

Possible Values: `count, -count`

## Response Codes

` 200 ``OK`

GameCenterMatchmakingRuleErrorsV1MetricResponse

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

### Getting rule results and errors

Get Boolean rule results

Get the results of a specific matchmaking rule that returns Boolean values.

Get numeric rule results

Get the results of a specific matchmaking rule that returns numeric values.

