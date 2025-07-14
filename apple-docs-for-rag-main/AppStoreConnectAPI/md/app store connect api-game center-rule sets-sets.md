

- App Store Connect API
- Game Center
-  Rule sets 

API Collection

# Rule sets

Manage the rule sets that you add matchmaking rules and teams to.

## Overview

The `rule set` resource represents a set of rules associated with a queue that Game Center applies to match requests in the queue. For more information, see Matchmaking rules in the GameKit framework.

## Topics

### Creating, modifying, and deleting rule sets

Create a rule set

Create a rule set to contain matchmaking rules and teams.

Modify a rule set

Update the attributes of a rule set.

Delete a rule set

Delete a rule set along with its matchmaking rules and teams.

### Reading rule set information

List all rule sets

Get information about all rule sets and their associated objects.

Read rule set information

Get information about a specific rule set and its related objects.

List queues in a rule set

Get information about queues that belong to a rule set.

List rules in a rule set

Get information about the rules in a rule set.

List teams in a rule set

Get information about the teams in a rule set.

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

object GameCenterMatchmakingRuleSet

The data structure that represents a rule set.

## See Also

### Matchmaking rules

Rules

Manage the matchmaking rules that Game Center uses to find players.

Expressions

Write expressions that query the match requests in a queue to find the best players for a match.

Queues

Manage the queues that contain matchmaking rule sets and that you submit match requests to.

Teams

Manage the teams that you add to matchmaking rule sets.

Testing

Test matchmaking rules using sample data.

Metrics

Analyze data about matchmaking rules.

