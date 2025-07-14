

- App Store Connect API
-  GameCenterMatchmakingRuleSet 

Object

# GameCenterMatchmakingRuleSet

The data structure that represents a rule set.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingRuleSet
```

## Properties

`attributes`

GameCenterMatchmakingRuleSet.Attributes

The attributes of the rule set.

`id`

`string`

 (Required) 

The unique identifier for the rule set.

`links`

ResourceLinks

`relationships`

GameCenterMatchmakingRuleSet.Relationships

The relationships to other objects belonging to the rule set.

`type`

`string`

 (Required) 

The type of resource.

Value: `gameCenterMatchmakingRuleSets`

## Topics

### Objects

object GameCenterMatchmakingRuleSet.Attributes

The attributes of the rule set.

object GameCenterMatchmakingRuleSet.Relationships

The relationships to other objects belonging to the rule set.

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

object GameCenterMatchmakingRulesResponse

The response body for endpoints that get multiple rules.

