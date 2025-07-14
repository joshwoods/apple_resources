

- App Store Connect API
- GameCenterMatchmakingRuleUpdateRequest
- GameCenterMatchmakingRuleUpdateRequest.Data
-  GameCenterMatchmakingRuleUpdateRequest.Data.Attributes 

Object

# GameCenterMatchmakingRuleUpdateRequest.Data.Attributes

The attributes of a rule that you modify.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingRuleUpdateRequest.Data.Attributes
```

## Properties

`description`

`string`

A human-readable description of the rule.

`expression`

`string`

Code that returns a Boolean or numeric value that the matchmaking rules algorithm executes to compare or filter match requests.

`weight`

`number`

A numeric value for the rule when `type` is either `DISTANCE` or `MATCH`.

