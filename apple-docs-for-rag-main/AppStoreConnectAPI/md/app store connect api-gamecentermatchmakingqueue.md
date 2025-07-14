

- App Store Connect API
-  GameCenterMatchmakingQueue 

Object

# GameCenterMatchmakingQueue

The data structure that represents a queue.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingQueue
```

## Properties

`attributes`

GameCenterMatchmakingQueue.Attributes

The attributes of the queue.

`id`

`string`

 (Required) 

The unique identifier for the rule.

`links`

ResourceLinks

The link representations of the object.

`relationships`

GameCenterMatchmakingQueue.Relationships

The relationships of the queue.

`type`

`string`

 (Required) 

The type of resource.

Value: `gameCenterMatchmakingQueues`

## Mentioned in 

App Store Connect API 3.2 release notes

## Topics

### Objects

object GameCenterMatchmakingQueue.Attributes

The attributes of the rule set.

object GameCenterMatchmakingQueue.Relationships

The rule sets associated with the queue.

## See Also

### Objects

object GameCenterMatchmakingQueueCreateRequest

The request body you use to create a queue.

object GameCenterMatchmakingQueueUpdateRequest

The request body you use to modify a queue.

object GameCenterMatchmakingQueueResponse

The response body for endpoints that create, modify, or get a single queue.

object GameCenterMatchmakingQueuesResponse

The response body for endpoints that get multiple queues.

