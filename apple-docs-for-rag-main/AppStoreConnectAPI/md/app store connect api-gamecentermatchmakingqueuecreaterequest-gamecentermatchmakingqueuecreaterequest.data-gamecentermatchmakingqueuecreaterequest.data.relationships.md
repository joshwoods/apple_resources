

- App Store Connect API
- GameCenterMatchmakingQueueCreateRequest
- GameCenterMatchmakingQueueCreateRequest.Data
-  GameCenterMatchmakingQueueCreateRequest.Data.Relationships 

Object

# GameCenterMatchmakingQueueCreateRequest.Data.Relationships

The rule sets that you include when creating a queue.

App Store Connect API 3.1+

``` source
object GameCenterMatchmakingQueueCreateRequest.Data.Relationships
```

## Properties

`experimentRuleSet`

GameCenterMatchmakingQueueCreateRequest.Data.Relationships.ExperimentRuleSet

The experimental rule set to test the associated rules with live match requests.

If you provide an experimental rule set, Game Center processes the match requests in the queue using both the experimental and the required rule set, except that it doesn’t return the results of the experimental rule set to clients.

Then compare the results of the experimental rule set with the production rule set using metrics, such as the List all queues and Read queue information endpoints.

`ruleSet`

GameCenterMatchmakingQueueCreateRequest.Data.Relationships.RuleSet

 (Required) 

The rule set to associate with this queue.

## Topics

### Objects

object GameCenterMatchmakingQueueCreateRequest.Data.Relationships.ExperimentRuleSet

An experimental rule set for testing this queue.

object GameCenterMatchmakingQueueCreateRequest.Data.Relationships.ExperimentRuleSet.Data

The data structure of the request body for an experimental rule set.

object GameCenterMatchmakingQueueCreateRequest.Data.Relationships.RuleSet

The rule set associated with the queue.

## See Also

### Objects

object GameCenterMatchmakingQueueCreateRequest.Data.Attributes

The attributes for a queue that you create.

