

- App Store Connect API
-  GameCenterMatchmakingTestRequestInlineCreate 

Object

# GameCenterMatchmakingTestRequestInlineCreate

A data structure that represents a sample match request for testing a rule set.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingTestRequestInlineCreate
```

## Properties

`attributes`

GameCenterMatchmakingTestRequestInlineCreate.Attributes

 (Required) 

The object attributes.

`id`

`string`

A unique identifier for the match request.

`relationships`

GameCenterMatchmakingTestRequestInlineCreate.Relationships

The object relationships.

`type`

`string`

 (Required) 

The type of resource object.

Value: `gameCenterMatchmakingTestRequests`

## Topics

### Objects

object GameCenterMatchmakingTestRequestInlineCreate.Attributes

The attributes for a sample match request.

object GameCenterMatchmakingTestRequestInlineCreate.Relationships

The relationships of a match request to other objects.

## See Also

### Objects

object GameCenterMatchmakingRuleSetTestCreateRequest

The request body for testing the rules in a rule set.

object GameCenterMatchmakingRuleSetTestResponse

The response body for testing a rule set.

object GameCenterMatchmakingRuleSetTest

The data structure that represents the results of testing a rule set.

object GameCenterMatchmakingTestPlayerPropertyInlineCreate

A resource object that represents a player’s properties when you create a request.

object GameCenterMatchmakingTeamAssignment

The data structure that represents the assignment of a player to a team.

object Location

A representation of a device location.

object Property

A representation of a game-specific property.

