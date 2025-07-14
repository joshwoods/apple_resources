

- App Store Connect API
-  GameCenterMatchmakingRulesResponse 

Object

# GameCenterMatchmakingRulesResponse

The response body for endpoints that get multiple rules.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingRulesResponse
```

## Properties

`data`

`[`GameCenterMatchmakingRule`]`

 (Required) 

The rules that the endpoint gets.

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

object GameCenterMatchmakingRuleSetsResponse

The response body for endpoints that get multiple rule sets.

object GameCenterMatchmakingRuleSet

The data structure that represents a rule set.

