

- App Store Connect API
-  Get classic match requests 

Web Service Endpoint

# Get classic match requests

Get match requests that don’t use matchmaking rules.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}/metrics/classicMatchmakingRequests
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the GameCenterDetail resource object. You can obtain this resource ID from the List Apps response.

## Query Parameters

`filter[result]`

`string`

The types of the match requests to include in the response.

Possible Values: `MATCHED, CANCELED, EXPIRED`

`granularity`

`string`

 (Required) 

The level of information you want in the response, specified as a time interval for the data collection, using the ISO 8601 format for durations.

Possible Values: `P1D, PT1H, PT15M`

`groupBy`

`[string]`

If `result`, organizes the match requests by outcome (matched, canceled, and expired).

Value: `result`

`limit`

`integer`

The maximum number of match requests to fetch.

Maximum: `200`

`sort`

`[string]`

Sort results by the specified order. For example, `count` sorts the results by decreasing number of players that Game Center finds.

Possible Values: `count, -count, averageSecondsInQueue, -averageSecondsInQueue, p50SecondsInQueue, -p50SecondsInQueue, p95SecondsInQueue, -p95SecondsInQueue`

## Response Codes

` 200 ``OK`

GameCenterMatchmakingAppRequestsV1MetricResponse

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

### Getting match request metrics

Get rule-based match requests

Get match requests that use matchmaking rules.

