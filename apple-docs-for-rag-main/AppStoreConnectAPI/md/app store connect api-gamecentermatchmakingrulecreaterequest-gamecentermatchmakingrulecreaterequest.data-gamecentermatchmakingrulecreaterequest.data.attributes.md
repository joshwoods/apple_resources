

- App Store Connect API
- GameCenterMatchmakingRuleCreateRequest
- GameCenterMatchmakingRuleCreateRequest.Data
-  GameCenterMatchmakingRuleCreateRequest.Data.Attributes 

Object

# GameCenterMatchmakingRuleCreateRequest.Data.Attributes

The attributes for a rule that you create.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingRuleCreateRequest.Data.Attributes
```

## Properties

`description`

`string`

 (Required) 

A human-readable description of the rule.

`expression`

`string`

 (Required) 

Code that returns a Boolean or numeric value that the matchmaking rules algorithm executes to compare or filter match requests.

`referenceName`

`string`

 (Required) 

A name for the rule that’s unique within the scope of its rule set.

`type`

`string`

 (Required) 

The type or category of the rule that determines the return value and properties available in the expression.

Possible Values: `COMPATIBLE, DISTANCE, MATCH, TEAM`

`weight`

`number`

A numeric value for the rule when `type` is either `DISTANCE` or `MATCH`.

## Discussion

The possible values for the `type` field are:

| `COMPATIBLE` | Rules that enforce constraints on two match requests and return a Boolean value.  For example, a rule that requires devices to run the same version of your game, or finds players that share a common language or game settings.  If you set the `type` field to `COMPATIBLE`, compare the two match requests in the `requests` array in your expression, as in:  `areCompatibleAppVersions(requests[0], requests[1])` |
|----|----|
| `DISTANCE` | Rules that evaluate the similarity of two match requests and return a numeric value between `0.0` and `1.0`.  For example, rules that compare the latency or distance between players and find players with the exact same language and region setting.  If you set the `type` field to `DISTANCE`, evaluate the two match requests in the `requests` array in your expression, as in:  `geoLatency(requests[0], requests[1])` |
| `MATCH` | Rules that evaluate properties across all compatible requests.  For example, rules that prefer match candidates with more players but allows less players after a period of time, compare the difference in skill levels of players to a desired skill level that’s a function of time, and find players that have compatible game configurations that loosen over time.  If you set the type field to `MATCH`, use the `requests` array in the expression to get all the compatible matches. |
| `TEAM` | Rules that evaluate the assignment of players to teams and return a Boolean value.  For example, rules that make the number of players on each team the same, balance the skill levels on each team for a fair match, and keep invited friends on the same team.  If you set the `type` field to `TEAM`, use the `teams` array to get all the teams associated with the rule set. |

## See Also

### Objects

object GameCenterMatchmakingRuleCreateRequest.Data.Relationships

The relationships to other objects that you include when creating a rule.

