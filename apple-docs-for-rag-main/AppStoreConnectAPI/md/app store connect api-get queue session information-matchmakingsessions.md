

- App Store Connect API
-  Get queue session information 

Web Service Endpoint

# Get queue session information

Get session information on a queue.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues/{id}/metrics/matchmakingSessions
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

The maximum number of sessions to include.

Maximum: `200`

`sort`

`[string]`

Sort sizes by the specified order. For example, `count` sorts the results by decreasing number of players that Game Center finds.

Possible Values: `count, -count, averagePlayerCount, -averagePlayerCount, p50PlayerCount, -p50PlayerCount, p95PlayerCount, -p95PlayerCount`

## Response Codes

` 200 ``OK`

GameCenterMatchmakingSessionsV1MetricResponse

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
GET https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues/0df9ae63-0328-4060-9afc-53e848e8c386/metrics/matchmakingSessions?granularity=PT15M
```

```
{
  "data": [
    {
      "type": "gameCenterMatchmakingSessions",
      "dataPoints": [
        {
          "start": "2023-10-10T23:30:00Z",
          "end": "2023-10-10T23:45:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T23:15:00Z",
          "end": "2023-10-10T23:30:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T23:00:00Z",
          "end": "2023-10-10T23:15:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T22:45:00Z",
          "end": "2023-10-10T23:00:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T22:30:00Z",
          "end": "2023-10-10T22:45:00Z",
          "values": {
            "count": 1,
            "p50PlayerCount": 2,
            "averagePlayerCount": 2,
            "p95PlayerCount": 2
          }
        },
        {
          "start": "2023-10-10T22:15:00Z",
          "end": "2023-10-10T22:30:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T22:00:00Z",
          "end": "2023-10-10T22:15:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T21:45:00Z",
          "end": "2023-10-10T22:00:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T21:30:00Z",
          "end": "2023-10-10T21:45:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T21:15:00Z",
          "end": "2023-10-10T21:30:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T21:00:00Z",
          "end": "2023-10-10T21:15:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T20:45:00Z",
          "end": "2023-10-10T21:00:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T20:30:00Z",
          "end": "2023-10-10T20:45:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T20:15:00Z",
          "end": "2023-10-10T20:30:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T20:00:00Z",
          "end": "2023-10-10T20:15:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T19:45:00Z",
          "end": "2023-10-10T20:00:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T19:30:00Z",
          "end": "2023-10-10T19:45:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T19:15:00Z",
          "end": "2023-10-10T19:30:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T19:00:00Z",
          "end": "2023-10-10T19:15:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T18:45:00Z",
          "end": "2023-10-10T19:00:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T18:30:00Z",
          "end": "2023-10-10T18:45:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T18:15:00Z",
          "end": "2023-10-10T18:30:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T18:00:00Z",
          "end": "2023-10-10T18:15:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T17:45:00Z",
          "end": "2023-10-10T18:00:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T17:30:00Z",
          "end": "2023-10-10T17:45:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T17:15:00Z",
          "end": "2023-10-10T17:30:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T17:00:00Z",
          "end": "2023-10-10T17:15:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T16:45:00Z",
          "end": "2023-10-10T17:00:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T16:30:00Z",
          "end": "2023-10-10T16:45:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T16:15:00Z",
          "end": "2023-10-10T16:30:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T16:00:00Z",
          "end": "2023-10-10T16:15:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        },
        {
          "start": "2023-10-10T15:45:00Z",
          "end": "2023-10-10T16:00:00Z",
          "values": {
            "count": 0,
            "p50PlayerCount": 0,
            "averagePlayerCount": 0,
            "p95PlayerCount": 0
          }
        }
      ],
      "granularity": 900
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/gameCenterMatchmakingQueues/0df9ae63-0328-4060-9afc-53e848e8c386/metrics/matchmakingSessions?granularity=PT15M"
  },
  "meta": {
    "paging": {
      "total": 1,
      "limit": 50
    }
  }
}

```

## See Also

### Getting queue information

Get queue size

Get the time that match requests are in a specific queue.

Get experimental queue size

Get the number of match requests that the queue processes using its experimental rule set.

Get match request time in queue

Get the match requests that a specific queue processes.

Get experimental match request time in queue

Get the match requests that a specific queue processes using its experimental rule set.

