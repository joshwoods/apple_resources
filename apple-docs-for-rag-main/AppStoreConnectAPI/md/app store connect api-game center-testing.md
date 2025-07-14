

- App Store Connect API
- Game Center
-  Testing 

API Collection

# Testing

Test matchmaking rules using sample data.

## Overview

Use the Testing APIs to apply matchmaking rules to sample match requests and player properties. For more information, see Testing matchmaking rules.

## Topics

### Applying rule sets to sample requests

Test a rule set

Apply the given rule set to the given sample match requests.

### Objects

object GameCenterMatchmakingRuleSetTestCreateRequest

The request body for testing the rules in a rule set.

object GameCenterMatchmakingRuleSetTestResponse

The response body for testing a rule set.

object GameCenterMatchmakingRuleSetTest

The data structure that represents the results of testing a rule set.

object GameCenterMatchmakingTestRequestInlineCreate

A data structure that represents a sample match request for testing a rule set.

object GameCenterMatchmakingTestPlayerPropertyInlineCreate

A resource object that represents a player’s properties when you create a request.

object GameCenterMatchmakingTeamAssignment

The data structure that represents the assignment of a player to a team.

object Location

A representation of a device location.

object Property

A representation of a game-specific property.

## See Also

### Matchmaking rules

Rules

Manage the matchmaking rules that Game Center uses to find players.

Expressions

Write expressions that query the match requests in a queue to find the best players for a match.

Rule sets

Manage the rule sets that you add matchmaking rules and teams to.

Queues

Manage the queues that contain matchmaking rule sets and that you submit match requests to.

Teams

Manage the teams that you add to matchmaking rule sets.

Metrics

Analyze data about matchmaking rules.

