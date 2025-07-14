

- App Store Connect API
- GameCenterMatchmakingQueueCreateRequest
- 
  - GameCenterMatchmakingQueueCreateRequest
- GameCenterMatchmakingQueueCreateRequest.Data
- GameCenterMatchmakingQueueCreateRequest.Data.Relationships
- GameCenterMatchmakingQueueCreateRequest.Data.Relationships.ExperimentRuleSet
-  GameCenterMatchmakingQueueCreateRequest.Data.Relationships.ExperimentRuleSet.Data 

Object

# GameCenterMatchmakingQueueCreateRequest.Data.Relationships.ExperimentRuleSet.Data

The data structure of the request body for an experimental rule set.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingQueueCreateRequest.Data.Relationships.ExperimentRuleSet.Data
```

## Properties

`id`

`string`

 (Required) 

The unique identifier for the rule set.

`type`

`string`

 (Required) 

The type of resource.

Value: `gameCenterMatchmakingRuleSets`

## See Also

### Objects

object GameCenterMatchmakingQueueCreateRequest.Data.Relationships.ExperimentRuleSet

An experimental rule set for testing this queue.

object GameCenterMatchmakingQueueCreateRequest.Data.Relationships.RuleSet

The rule set associated with the queue.

