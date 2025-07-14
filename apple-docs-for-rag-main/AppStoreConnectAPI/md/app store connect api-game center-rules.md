

- App Store Connect API
- Game Center
-  Rules 

API Collection

# Rules

Manage the matchmaking rules that Game Center uses to find players.

## Overview

The `rules` resource represents a matchmaking rule that Game Center applies to match requests in a queue.

With matchmaking rules, you have finer control over automatch of players to fill empty slots in a match request. For example, use matchmaking rules to find compatible players and assign them to teams using game-specific information, such as skill level and other criteria. During development, you use the matchmaking rules APIs to upload your rules to the Game Center server. In your game code, you configure match requests to use your set of matchmaking rules. When you submit the match requests, Game Center applies your rules to the collective match requests from multiple game instances in the queue to fill the empty slots.

For more information, see Matchmaking rules in the GameKit framework.

## Topics

### Creating, modifying, and deleting rules

Create a rule

Add a matchmaking rule to a rule set.

Modify a rule

Update a specific matchmaking rule in a rule set.

Delete a rule

Delete a matchmaking rule in a rule set.

### Objects

object GameCenterMatchmakingRuleCreateRequest

The request body you use to create a rule.

object GameCenterMatchmakingRuleUpdateRequest

The request body you use to modify a rule.

object GameCenterMatchmakingRuleResponse

The response body for endpoints that create or modify a rule.

object GameCenterMatchmakingRule

The data structure that represents a matchmaking rule.

## See Also

### Matchmaking rules

Expressions

Write expressions that query the match requests in a queue to find the best players for a match.

Rule sets

Manage the rule sets that you add matchmaking rules and teams to.

Queues

Manage the queues that contain matchmaking rule sets and that you submit match requests to.

Teams

Manage the teams that you add to matchmaking rule sets.

Testing

Test matchmaking rules using sample data.

Metrics

Analyze data about matchmaking rules.

