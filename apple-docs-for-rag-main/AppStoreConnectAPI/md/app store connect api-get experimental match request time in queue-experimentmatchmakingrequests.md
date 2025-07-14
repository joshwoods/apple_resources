

- App Store Connect API
-  Get experimental match request time in queue 

Web Service Endpoint

# Get experimental match request time in queue

Get the match requests that a specific queue processes using its experimental rule set.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues/{id}/metrics/experimentMatchmakingRequests
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the queue.

## Query Parameters

`filter[gameCenterDetail]`

`string`

The fields of the queues to include in the response.

`filter[result]`

`string`

The types of match requests to include in the response.

Possible Values: `MATCHED, CANCELED, EXPIRED`

`granularity`

`string`

 (Required) 

The level of information you want in the response, specified as a time interval for the data collection, using the ISO 8601 format for durations.

Possible Values: `P1D, PT1H, PT15M`

`groupBy`

`[string]`

Group match requests by result.

Possible Values: `result, gameCenterDetail`

`limit`

`integer`

The maximum number of match requests to include.

Maximum: `200`

`sort`

`[string]`

Sort sizes by the specified order. For example, `count` sorts the results by decreasing number of players that Game Center finds.

Possible Values: `count, -count, averageSecondsInQueue, -averageSecondsInQueue, p50SecondsInQueue, -p50SecondsInQueue, p95SecondsInQueue, -p95SecondsInQueue`

## Response Codes

` 200 ``OK`

GameCenterMatchmakingQueueRequestsV1MetricResponse

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

### Getting queue information

Get queue size

Get the time that match requests are in a specific queue.

Get experimental queue size

Get the number of match requests that the queue processes using its experimental rule set.

Get match request time in queue

Get the match requests that a specific queue processes.

Get queue session information

Get session information on a queue.

