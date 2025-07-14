

- App Store Connect API
-  GameCenterMatchmakingQueuesResponse 

Object

# GameCenterMatchmakingQueuesResponse

The response body for endpoints that get multiple queues.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingQueuesResponse
```

## Properties

`data`

`[`GameCenterMatchmakingQueue`]`

 (Required) 

The queues that the endpoint fetches.

`included`

`[`GameCenterMatchmakingRuleSet`]`

The rule sets included in the response.

`links`

PagedDocumentLinks

 (Required) 

The link representations of the response.

`meta`

PagingInformation

## See Also

### Objects

object GameCenterMatchmakingQueueCreateRequest

The request body you use to create a queue.

object GameCenterMatchmakingQueueUpdateRequest

The request body you use to modify a queue.

object GameCenterMatchmakingQueueResponse

The response body for endpoints that create, modify, or get a single queue.

object GameCenterMatchmakingQueue

The data structure that represents a queue.

