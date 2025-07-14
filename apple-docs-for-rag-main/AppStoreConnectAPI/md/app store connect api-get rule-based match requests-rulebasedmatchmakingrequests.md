

- App Store Connect API
-  Get rule-based match requests 

Web Service Endpoint

# Get rule-based match requests

Get match requests that use matchmaking rules.

App Store Connect API 3.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterDetails/{id}/metrics/ruleBasedMatchmakingRequests
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

If `result`, organizes the match requests by type (`MATCHED`, `CANCELED`, and `EXPIRED`).

Value: `result`

`limit`

`integer`

The maximum number of match requests to fetch.

Maximum: `200`

`sort`

`[string]`

Sorts the match request by count or duration in the queue. For example, `count` sorts the results by decreasing number of players that Game Center finds.

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

## Discussion

### Example Request and Response

- Request
- Response

```
GET /v1/gameCenterDetails/8fb73d41-1ca1-1cbf-2538-9df424beb10b/metrics/ruleBasedMatchmakingRequests?granularity=PT15M
```

```
{
  “data”: [
    {
      “type”: “gameCenterMatchmakingAppRequests”,
      “dataPoints”: [
        {
          “start”: “2023-10-05T04:00:00Z”,
          “end”: “2023-10-05T04:15:00Z”,
          “values”: {
            “averageSecondsInQueue”: 2.9630714285714284,
            “p95SecondsInQueue”: 3.838,
            “count”: 14,
            “p50SecondsInQueue”: 3.36
          }
        },
        {
          “start”: “2023-10-05T03:45:00Z”,
          “end”: “2023-10-05T04:00:00Z”,
          “values”: {
            “averageSecondsInQueue”: 87.95857142857143,
            “p95SecondsInQueue”: 302.343,
            “count”: 14,
            “p50SecondsInQueue”: 3.435
          }
        },
        {
          “start”: “2023-10-05T03:30:00Z”,
          “end”: “2023-10-05T03:45:00Z”,
          “values”: {
            “averageSecondsInQueue”: 3.7325,
            “p95SecondsInQueue”: 3.984,
            “count”: 4,
            “p50SecondsInQueue”: 3.818
          }
        },
        {
          “start”: “2023-10-05T03:15:00Z”,
          “end”: “2023-10-05T03:30:00Z”,
          “values”: {
            “averageSecondsInQueue”: 301.53325,
            “p95SecondsInQueue”: 302.924,
            “count”: 4,
            “p50SecondsInQueue”: 302.62
          }
        },
        {
          “start”: “2023-10-05T03:00:00Z”,
          “end”: “2023-10-05T03:15:00Z”,
          “values”: {
            “averageSecondsInQueue”: 2.883714285714286,
            “p95SecondsInQueue”: 3.53,
            “count”: 14,
            “p50SecondsInQueue”: 3.346
          }
        },
        {
          “start”: “2023-10-05T02:45:00Z”,
          “end”: “2023-10-05T03:00:00Z”,
          “values”: {
            “averageSecondsInQueue”: 87.926,
            “p95SecondsInQueue”: 302.848,
            “count”: 14,
            “p50SecondsInQueue”: 3.197
          }
        },
        {
          “start”: “2023-10-05T02:30:00Z”,
          “end”: “2023-10-05T02:45:00Z”,
          “values”: {
            “averageSecondsInQueue”: 3.42825,
            “p95SecondsInQueue”: 3.66,
            “count”: 4,
            “p50SecondsInQueue”: 3.503
          }
        },
        {
          “start”: “2023-10-05T02:15:00Z”,
          “end”: “2023-10-05T02:30:00Z”,
          “values”: {
            “averageSecondsInQueue”: 300.98025,
            “p95SecondsInQueue”: 301.383,
            “count”: 4,
            “p50SecondsInQueue”: 301.108
          }
        },
        {
          “start”: “2023-10-05T02:00:00Z”,
          “end”: “2023-10-05T02:15:00Z”,
          “values”: {
            “averageSecondsInQueue”: 2.928,
            “p95SecondsInQueue”: 3.777,
            “count”: 14,
            “p50SecondsInQueue”: 3.29
          }
        },
        {
          “start”: “2023-10-05T01:45:00Z”,
          “end”: “2023-10-05T02:00:00Z”,
          “values”: {
            “averageSecondsInQueue”: 87.93171428571429,
            “p95SecondsInQueue”: 302.445,
            “count”: 14,
            “p50SecondsInQueue”: 3.242
          }
        },
        {
          “start”: “2023-10-05T01:30:00Z”,
          “end”: “2023-10-05T01:45:00Z”,
          “values”: {
            “averageSecondsInQueue”: 3.1195,
            “p95SecondsInQueue”: 3.34,
            “count”: 4,
            “p50SecondsInQueue”: 3.196
          }
        },
        {
          “start”: “2023-10-05T01:15:00Z”,
          “end”: “2023-10-05T01:30:00Z”,
          “values”: {
            “averageSecondsInQueue”: 301.0555,
            “p95SecondsInQueue”: 302.572,
            “count”: 4,
            “p50SecondsInQueue”: 301.148
          }
        },
        {
          “start”: “2023-10-05T01:00:00Z”,
          “end”: “2023-10-05T01:15:00Z”,
          “values”: {
            “averageSecondsInQueue”: 3.0154285714285716,
            “p95SecondsInQueue”: 3.678,
            “count”: 14,
            “p50SecondsInQueue”: 3.484
          }
        },
        {
          “start”: “2023-10-05T00:45:00Z”,
          “end”: “2023-10-05T01:00:00Z”,
          “values”: {
            “averageSecondsInQueue”: 88.19257142857144,
            “p95SecondsInQueue”: 302.78,
            “count”: 14,
            “p50SecondsInQueue”: 3.413
          }
        },
        {
          “start”: “2023-10-05T00:30:00Z”,
          “end”: “2023-10-05T00:45:00Z”,
          “values”: {
            “averageSecondsInQueue”: 3.109,
            “p95SecondsInQueue”: 3.387,
            “count”: 4,
            “p50SecondsInQueue”: 3.182
          }
        },
        {
          “start”: “2023-10-05T00:15:00Z”,
          “end”: “2023-10-05T00:30:00Z”,
          “values”: {
            “averageSecondsInQueue”: 301.06625,
            “p95SecondsInQueue”: 302.979,
            “count”: 4,
            “p50SecondsInQueue”: 300.68
          }
        },
        {
          “start”: “2023-10-05T00:00:00Z”,
          “end”: “2023-10-05T00:15:00Z”,
          “values”: {
            “averageSecondsInQueue”: 2.8656428571428574,
            “p95SecondsInQueue”: 3.663,
            “count”: 14,
            “p50SecondsInQueue”: 3.237
          }
        },
        {
          “start”: “2023-10-04T23:45:00Z”,
          “end”: “2023-10-05T00:00:00Z”,
          “values”: {
            “averageSecondsInQueue”: 88.13835714285715,
            “p95SecondsInQueue”: 303.037,
            “count”: 14,
            “p50SecondsInQueue”: 3.409
          }
        },
        {
          “start”: “2023-10-04T23:30:00Z”,
          “end”: “2023-10-04T23:45:00Z”,
          “values”: {
            “averageSecondsInQueue”: 3.0285,
            “p95SecondsInQueue”: 3.312,
            “count”: 4,
            “p50SecondsInQueue”: 3.152
          }
        },
        {
          “start”: “2023-10-04T23:15:00Z”,
          “end”: “2023-10-04T23:30:00Z”,
          “values”: {
            “averageSecondsInQueue”: 0,
            “p95SecondsInQueue”: 0,
            “count”: 0,
            “p50SecondsInQueue”: 0
          }
        },
        {
          “start”: “2023-10-04T23:00:00Z”,
          “end”: “2023-10-04T23:15:00Z”,
          “values”: {
            “averageSecondsInQueue”: 0,
            “p95SecondsInQueue”: 0,
            “count”: 0,
            “p50SecondsInQueue”: 0
          }
        },
        {
          “start”: “2023-10-04T22:45:00Z”,
          “end”: “2023-10-04T23:00:00Z”,
          “values”: {
            “averageSecondsInQueue”: 0,
            “p95SecondsInQueue”: 0,
            “count”: 0,
            “p50SecondsInQueue”: 0
          }
        },
        {
          “start”: “2023-10-04T22:30:00Z”,
          “end”: “2023-10-04T22:45:00Z”,
          “values”: {
            “averageSecondsInQueue”: 0,
            “p95SecondsInQueue”: 0,
            “count”: 0,
            “p50SecondsInQueue”: 0
          }
        },
        {
          “start”: “2023-10-04T22:15:00Z”,
          “end”: “2023-10-04T22:30:00Z”,
          “values”: {
            “averageSecondsInQueue”: 0,
            “p95SecondsInQueue”: 0,
            “count”: 0,
            “p50SecondsInQueue”: 0
          }
        },
        {
          “start”: “2023-10-04T22:00:00Z”,
          “end”: “2023-10-04T22:15:00Z”,
          “values”: {
            “averageSecondsInQueue”: 0,
            “p95SecondsInQueue”: 0,
            “count”: 0,
            “p50SecondsInQueue”: 0
          }
        },
        {
          “start”: “2023-10-04T21:45:00Z”,
          “end”: “2023-10-04T22:00:00Z”,
          “values”: {
            “averageSecondsInQueue”: 0,
            “p95SecondsInQueue”: 0,
            “count”: 0,
            “p50SecondsInQueue”: 0
          }
        },
        {
          “start”: “2023-10-04T21:30:00Z”,
          “end”: “2023-10-04T21:45:00Z”,
          “values”: {
            “averageSecondsInQueue”: 0,
            “p95SecondsInQueue”: 0,
            “count”: 0,
            “p50SecondsInQueue”: 0
          }
        },
        {
          “start”: “2023-10-04T21:15:00Z”,
          “end”: “2023-10-04T21:30:00Z”,
          “values”: {
            “averageSecondsInQueue”: 301.37775,
            “p95SecondsInQueue”: 302.627,
            “count”: 4,
            “p50SecondsInQueue”: 302.513
          }
        },
        {
          “start”: “2023-10-04T21:00:00Z”,
          “end”: “2023-10-04T21:15:00Z”,
          “values”: {
            “averageSecondsInQueue”: 2.8602857142857143,
            “p95SecondsInQueue”: 3.528,
            “count”: 14,
            “p50SecondsInQueue”: 3.318
          }
        },
        {
          “start”: “2023-10-04T20:45:00Z”,
          “end”: “2023-10-04T21:00:00Z”,
          “values”: {
            “averageSecondsInQueue”: 87.86357142857143,
            “p95SecondsInQueue”: 302.205,
            “count”: 14,
            “p50SecondsInQueue”: 3.173
          }
        },
        {
          “start”: “2023-10-04T20:30:00Z”,
          “end”: “2023-10-04T20:45:00Z”,
          “values”: {
            “averageSecondsInQueue”: 3.11125,
            “p95SecondsInQueue”: 3.359,
            “count”: 4,
            “p50SecondsInQueue”: 3.186
          }
        },
        {
          “start”: “2023-10-04T20:15:00Z”,
          “end”: “2023-10-04T20:30:00Z”,
          “values”: {
            “averageSecondsInQueue”: 0,
            “p95SecondsInQueue”: 0,
            “count”: 0,
            “p50SecondsInQueue”: 0
          }
        }
      ],
      “dimensions”: {
        “result”: {
          “links”: {
            “groupBy”: “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/8fb73d41-1ca1-1cbf-2538-9df424beb10b/metrics/ruleBasedMatchmakingRequests?groupBy=result”
          }
        }
      },
      “granularity”: 900
    }
  ],
  “links”: {
    “self”: “https://api.appstoreconnect.apple.com/v1/gameCenterDetails/8fb73d41-1ca1-1cbf-2538-9df424beb10b/metrics/ruleBasedMatchmakingRequests?granularity=PT15M”
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

### Getting match request metrics

Get classic match requests

Get match requests that don’t use matchmaking rules.

