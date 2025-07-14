

- App Store Connect API
- GameCenterMatchmakingRule
-  GameCenterMatchmakingRule.Attributes 

Object

# GameCenterMatchmakingRule.Attributes

The attributes of a matchmaking rule.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingRule.Attributes
```

## Properties

`description`

`string`

A human-readable description of the rule.

`expression`

`string`

Code that returns a Boolean or numeric value that the matchmaking rules algorithm executes to compare or filter match requests.

`referenceName`

`string`

A name for the rule that’s unique within the scope of its rule set.

`type`

`string`

The type or category of the rule that determines the return value and properties available in the expression.

Possible Values: `COMPATIBLE, DISTANCE, MATCH, TEAM`

`weight`

`number`

A numeric value for the rule when `type` is either `DISTANCE` or `MATCH`.

