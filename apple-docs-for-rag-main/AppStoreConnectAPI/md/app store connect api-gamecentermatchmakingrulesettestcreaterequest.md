

- App Store Connect API
-  GameCenterMatchmakingRuleSetTestCreateRequest 

Object

# GameCenterMatchmakingRuleSetTestCreateRequest

The request body for testing the rules in a rule set.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingRuleSetTestCreateRequest
```

## Properties

`data`

GameCenterMatchmakingRuleSetTestCreateRequest.Data

 (Required) 

The data structure for the request body.

`included`

`[*]`

The resource objects that Game Center uses in the test.

Possible types: GameCenterMatchmakingTestPlayerPropertyInlineCreate`, `GameCenterMatchmakingTestRequestInlineCreate

## Topics

### Objects

object GameCenterMatchmakingRuleSetTestCreateRequest.Data

The data structure of the request body for testing a rule set.

## See Also

### Objects

object GameCenterMatchmakingRuleSetTestResponse

The response body for testing a rule set.

object GameCenterMatchmakingRuleSetTest

The data structure that represents the results of testing a rule set.

object GameCenterMatchmakingTestRequestInlineCreate

A data structure that represents a sample match request for testing a rule set.

object GameCenterMatchmakingTestPlayerPropertyInlineCreate

A resource object that represents a player’s properties when you create a request.

object GameCenterMatchmakingTeamAssignment

The data structure that represents the assignment of a player to a team.

object Location

A representation of a device location.

object Property

A representation of a game-specific property.

