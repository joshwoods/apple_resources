

- App Store Connect API
- GameCenterMatchmakingTestRequestInlineCreate
- GameCenterMatchmakingTestRequestInlineCreate.Relationships
- GameCenterMatchmakingTestRequestInlineCreate.Relationships.MatchmakingPlayerProperties
-  GameCenterMatchmakingTestRequestInlineCreate.Relationships.MatchmakingPlayerProperties.Data 

Object

# GameCenterMatchmakingTestRequestInlineCreate.Relationships.MatchmakingPlayerProperties.Data

The resource object for the game-specific properties of a match request.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingTestRequestInlineCreate.Relationships.MatchmakingPlayerProperties.Data
```

## Properties

`id`

`string`

 (Required) 

The identifier for a GameCenterMatchmakingTestPlayerPropertyInlineCreate resource object that you add to the `included` field of the request.

`type`

`string`

 (Required) 

The type of resource object.

Value: `gameCenterMatchmakingTestPlayerProperties`

