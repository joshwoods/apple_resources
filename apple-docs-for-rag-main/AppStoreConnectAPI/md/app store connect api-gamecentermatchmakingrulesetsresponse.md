

- App Store Connect API
-  GameCenterMatchmakingRuleSetsResponse 

Object

# GameCenterMatchmakingRuleSetsResponse

The response body for endpoints that get multiple rule sets.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingRuleSetsResponse
```

## Properties

`data`

`[`GameCenterMatchmakingRuleSet`]`

 (Required) 

The rule sets that an endpoint gets.

`included`

`[*]`

The related objects included in the response.

Possible types: GameCenterMatchmakingTeam`, `GameCenterMatchmakingRule`, `GameCenterMatchmakingQueue

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object GameCenterMatchmakingRuleSetCreateRequest

The request body you use to create a rule set.

object GameCenterMatchmakingRuleSetUpdateRequest

The request body you use to modify a rule set.

object GameCenterMatchmakingRuleSetResponse

The response body for endpoints that create, modify, or get a single rule.

object GameCenterMatchmakingRulesResponse

The response body for endpoints that get multiple rules.

object GameCenterMatchmakingRuleSet

The data structure that represents a rule set.

