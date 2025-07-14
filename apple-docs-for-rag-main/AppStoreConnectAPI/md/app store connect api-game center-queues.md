

- App Store Connect API
- Game Center
-  Queues 

API Collection

# Queues

Manage the queues that contain matchmaking rule sets and that you submit match requests to.

## Overview

The `queue` resource represents a queue of match requests that Game Center applies the associated set of matchmaking rules to. For more information, see Matchmaking rules in the GameKit framework.

## Topics

### Creating, modifying, and deleting queues

Create a queue

Create a queue and add it to a rule set.

Modify a queue

Update the properties of a specific queue.

Delete a queue

Delete a specific queue in a rule set.

### Reading queue information

List all queues

Get information about all queues.

Read queue information

Get information about a specific queue and its related objects.

### Objects

object GameCenterMatchmakingQueueCreateRequest

The request body you use to create a queue.

object GameCenterMatchmakingQueueUpdateRequest

The request body you use to modify a queue.

object GameCenterMatchmakingQueueResponse

The response body for endpoints that create, modify, or get a single queue.

object GameCenterMatchmakingQueuesResponse

The response body for endpoints that get multiple queues.

object GameCenterMatchmakingQueue

The data structure that represents a queue.

## See Also

### Matchmaking rules

Rules

Manage the matchmaking rules that Game Center uses to find players.

Expressions

Write expressions that query the match requests in a queue to find the best players for a match.

Rule sets

Manage the rule sets that you add matchmaking rules and teams to.

Teams

Manage the teams that you add to matchmaking rule sets.

Testing

Test matchmaking rules using sample data.

Metrics

Analyze data about matchmaking rules.

