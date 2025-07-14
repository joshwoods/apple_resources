

- App Store Connect API
- Game Center
-  Teams 

API Collection

# Teams

Manage the teams that you add to matchmaking rule sets.

## Overview

The `team` resource represents an optional game-specific team that Game Center assigns to players using team rules. For more information, see Assigning players to teams using rules.

## Topics

### Creating, modifying, and deleting teams

Create a team

Add a game-specific team to a rule set.

Modify a team

Update a specific team in a rule set.

Delete a team

Delete a game-specific team in a rule set.

### Objects

object GameCenterMatchmakingTeamCreateRequest

The request body you use to create a team.

object GameCenterMatchmakingTeamUpdateRequest

The request body you use to modify a team.

object GameCenterMatchmakingTeamResponse

The response body for endpoints that create or modify a team.

object GameCenterMatchmakingTeamsResponse

The response body for endpoints that get multiple teams.

object GameCenterMatchmakingTeam

The data structure that represents a team.

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

Testing

Test matchmaking rules using sample data.

Metrics

Analyze data about matchmaking rules.

