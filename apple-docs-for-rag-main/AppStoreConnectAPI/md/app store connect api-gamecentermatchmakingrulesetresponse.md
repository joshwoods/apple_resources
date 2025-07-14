

- App Store Connect API
-  GameCenterMatchmakingRuleSetResponse 

Object

# GameCenterMatchmakingRuleSetResponse

The response body for endpoints that create, modify, or get a single rule.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingRuleSetResponse
```

## Properties

`data`

GameCenterMatchmakingRuleSet

 (Required) 

The rule set that you create, modify, or get.

`included`

`[*]`

The related objects included in the response.

Possible types: GameCenterMatchmakingTeam`, `GameCenterMatchmakingRule`, `GameCenterMatchmakingQueue

`links`

DocumentLinks

 (Required) 

## See Also

### Objects

object GameCenterMatchmakingRuleSetCreateRequest

The request body you use to create a rule set.

object GameCenterMatchmakingRuleSetUpdateRequest

The request body you use to modify a rule set.

object GameCenterMatchmakingRuleSetsResponse

The response body for endpoints that get multiple rule sets.

object GameCenterMatchmakingRulesResponse

The response body for endpoints that get multiple rules.

object GameCenterMatchmakingRuleSet

The data structure that represents a rule set.

