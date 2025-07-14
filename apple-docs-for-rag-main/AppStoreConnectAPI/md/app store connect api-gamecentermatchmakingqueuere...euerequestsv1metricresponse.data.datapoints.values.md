

- App Store Connect API
- GameCenterMatchmakingQueueRequestsV1MetricResponse
- GameCenterMatchmakingQueueRequestsV1MetricResponse.Data
- GameCenterMatchmakingQueueRequestsV1MetricResponse.Data.DataPoints
-  GameCenterMatchmakingQueueRequestsV1MetricResponse.Data.DataPoints.Values 

Object

# GameCenterMatchmakingQueueRequestsV1MetricResponse.Data.DataPoints.Values

The values of the data points.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingQueueRequestsV1MetricResponse.Data.DataPoints.Values
```

## Properties

`averageSecondsInQueue`

`number`

The average seconds that match requests are in the queue.

`count`

`integer`

The number of match requests in the queue.

`p50SecondsInQueue`

`number`

The number of seconds the 50th percentile of the match requests are in the queue.

`p95SecondsInQueue`

`number`

The number of seconds that the 95th percentile of the match requests are in the queue.

