

- App Store Connect API
-  GameCenterMatchmakingQueueResponse 

Object

# GameCenterMatchmakingQueueResponse

The response body for endpoints that create, modify, or get a single queue.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingQueueResponse
```

## Properties

`data`

GameCenterMatchmakingQueue

 (Required) 

The queue that you create, modify, or get.

`included`

`[`GameCenterMatchmakingRuleSet`]`

The rule sets included in the response.

`links`

DocumentLinks

 (Required) 

The link representations of the response.

## See Also

### Objects

object GameCenterMatchmakingQueueCreateRequest

The request body you use to create a queue.

object GameCenterMatchmakingQueueUpdateRequest

The request body you use to modify a queue.

object GameCenterMatchmakingQueuesResponse

The response body for endpoints that get multiple queues.

object GameCenterMatchmakingQueue

The data structure that represents a queue.

