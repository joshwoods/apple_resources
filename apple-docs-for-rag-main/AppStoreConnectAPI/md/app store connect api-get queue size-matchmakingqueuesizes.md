

- App Store Connect API
-  Get queue size 

Web Service Endpoint

# Get queue size

Get the time that match requests are in a specific queue.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingQueueSizes
```

## Path Parameters

`id`

`string`

 (Required) 

The unique identifier for the queue.

## Query Parameters

`granularity`

`string`

 (Required) 

The level of information you want in the response, specified as a time interval for the data collection, using the ISO 8601 format for durations.

Possible Values: `P1D, PT1H, PT15M`

`limit`

`integer`

The maximum number of queue size metrics to include.

Maximum: `200`

`sort`

`[string]`

Sort sizes by the specified order. For example, `count` sorts the results by decreasing number of players that Game Center finds.

Possible Values: `count, -count, averageNumberOfRequests, -averageNumberOfRequests, p50NumberOfRequests, -p50NumberOfRequests, p95NumberOfRequests, -p95NumberOfRequests`

## Response Codes

` 200 ``OK`

GameCenterMatchmakingQueueSizesV1MetricResponse

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

## Discussion

### Example Request and Response

- Request
- Response

```
GET https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues/02a62ecf-addf-48dc-a483-db6db43c574c/metrics/matchmakingQueueSizes?granularity=PT15M/gameCenterMatchmakingQueues/532ad9c0-1a28-4536-ad57-33213bcc0a29/metrics/
```

```
{
  “data”: [
    {
      “type”: “gameCenterMatchmakingQueueSizes”,
      “dataPoints”: [
        {
          “start”: “2023-10-07T02:15:00Z”,
          “end”: “2023-10-07T02:30:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-07T02:00:00Z”,
          “end”: “2023-10-07T02:15:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-07T01:45:00Z”,
          “end”: “2023-10-07T02:00:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.01010101010101,
            “p95NumberOfRequests”: 2,
            “count”: 99
          }
        },
        {
          “start”: “2023-10-07T01:30:00Z”,
          “end”: “2023-10-07T01:45:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-07T01:15:00Z”,
          “end”: “2023-10-07T01:30:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.0202020202020203,
            “p95NumberOfRequests”: 2,
            “count”: 99
          }
        },
        {
          “start”: “2023-10-07T01:00:00Z”,
          “end”: “2023-10-07T01:15:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-07T00:45:00Z”,
          “end”: “2023-10-07T01:00:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.01010101010101,
            “p95NumberOfRequests”: 2,
            “count”: 99
          }
        },
        {
          “start”: “2023-10-07T00:30:00Z”,
          “end”: “2023-10-07T00:45:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-07T00:15:00Z”,
          “end”: “2023-10-07T00:30:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.01010101010101,
            “p95NumberOfRequests”: 2,
            “count”: 99
          }
        },
        {
          “start”: “2023-10-07T00:00:00Z”,
          “end”: “2023-10-07T00:15:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-06T23:45:00Z”,
          “end”: “2023-10-07T00:00:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.0202020202020203,
            “p95NumberOfRequests”: 2,
            “count”: 99
          }
        },
        {
          “start”: “2023-10-06T23:30:00Z”,
          “end”: “2023-10-06T23:45:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-06T23:15:00Z”,
          “end”: “2023-10-06T23:30:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 1.99,
            “p95NumberOfRequests”: 2,
            “count”: 100
          }
        },
        {
          “start”: “2023-10-06T23:00:00Z”,
          “end”: “2023-10-06T23:15:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-06T22:45:00Z”,
          “end”: “2023-10-06T23:00:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.01010101010101,
            “p95NumberOfRequests”: 2,
            “count”: 99
          }
        },
        {
          “start”: “2023-10-06T22:30:00Z”,
          “end”: “2023-10-06T22:45:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-06T22:15:00Z”,
          “end”: “2023-10-06T22:30:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.01010101010101,
            “p95NumberOfRequests”: 2,
            “count”: 99
          }
        },
        {
          “start”: “2023-10-06T22:00:00Z”,
          “end”: “2023-10-06T22:15:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-06T21:45:00Z”,
          “end”: “2023-10-06T22:00:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.01010101010101,
            “p95NumberOfRequests”: 2,
            “count”: 99
          }
        },
        {
          “start”: “2023-10-06T21:30:00Z”,
          “end”: “2023-10-06T21:45:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-06T21:15:00Z”,
          “end”: “2023-10-06T21:30:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.020408163265306,
            “p95NumberOfRequests”: 2,
            “count”: 98
          }
        },
        {
          “start”: “2023-10-06T21:00:00Z”,
          “end”: “2023-10-06T21:15:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-06T20:45:00Z”,
          “end”: “2023-10-06T21:00:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.01010101010101,
            “p95NumberOfRequests”: 2,
            “count”: 99
          }
        },
        {
          “start”: “2023-10-06T20:30:00Z”,
          “end”: “2023-10-06T20:45:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-06T20:15:00Z”,
          “end”: “2023-10-06T20:30:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.020408163265306,
            “p95NumberOfRequests”: 2,
            “count”: 98
          }
        },
        {
          “start”: “2023-10-06T20:00:00Z”,
          “end”: “2023-10-06T20:15:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-06T19:45:00Z”,
          “end”: “2023-10-06T20:00:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.0202020202020203,
            “p95NumberOfRequests”: 2,
            “count”: 99
          }
        },
        {
          “start”: “2023-10-06T19:30:00Z”,
          “end”: “2023-10-06T19:45:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-06T19:15:00Z”,
          “end”: “2023-10-06T19:30:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2,
            “p95NumberOfRequests”: 2,
            “count”: 99
          }
        },
        {
          “start”: “2023-10-06T19:00:00Z”,
          “end”: “2023-10-06T19:15:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        },
        {
          “start”: “2023-10-06T18:45:00Z”,
          “end”: “2023-10-06T19:00:00Z”,
          “values”: {
            “p50NumberOfRequests”: 2,
            “averageNumberOfRequests”: 2.020408163265306,
            “p95NumberOfRequests”: 2,
            “count”: 98
          }
        },
        {
          “start”: “2023-10-06T18:30:00Z”,
          “end”: “2023-10-06T18:45:00Z”,
          “values”: {
            “p50NumberOfRequests”: 0,
            “averageNumberOfRequests”: 0,
            “p95NumberOfRequests”: 0,
            “count”: 0
          }
        }
      ],
      “granularity”: 900
    }
  ],
  “links”: {
    “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues/02a62ecf-addf-48dc-a483-db6db43c574c/metrics/matchmakingQueueSizes?granularity=PT15M”
  },
  “meta”: {
    “paging”: {
      “total”: 1,
      “limit”: 50
    }
  }
}
```

## See Also

### Getting queue information

Get experimental queue size

Get the number of match requests that the queue processes using its experimental rule set.

Get match request time in queue

Get the match requests that a specific queue processes.

Get experimental match request time in queue

Get the match requests that a specific queue processes using its experimental rule set.

Get queue session information

Get session information on a queue.

