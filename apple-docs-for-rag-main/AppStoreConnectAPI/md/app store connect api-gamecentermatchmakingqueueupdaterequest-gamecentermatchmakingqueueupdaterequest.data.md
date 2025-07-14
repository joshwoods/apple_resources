

- App Store Connect API
- GameCenterMatchmakingQueueUpdateRequest
-  GameCenterMatchmakingQueueUpdateRequest.Data 

Object

# GameCenterMatchmakingQueueUpdateRequest.Data

The data structure of the request body you use to modify a queue.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingQueueUpdateRequest.Data
```

## Properties

`attributes`

GameCenterMatchmakingQueueUpdateRequest.Data.Attributes

`id`

`string`

 (Required) 

The unique identifier for the queue.

`relationships`

GameCenterMatchmakingQueueUpdateRequest.Data.Relationships

`type`

`string`

 (Required) 

The type of resource.

Value: `gameCenterMatchmakingQueues`

## Topics

### Objects

object GameCenterMatchmakingQueueUpdateRequest.Data.Attributes

The attributes for a queue that you modify.

object GameCenterMatchmakingQueueUpdateRequest.Data.Relationships

The rule sets related to the queue.

