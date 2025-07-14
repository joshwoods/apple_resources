

- App Store Connect API
- Game Center
-  Metrics 

API Collection

# Metrics

Analyze data about matchmaking rules.

## Overview

Use the Metrics APIs to diagnose performance and other issues with matchmaking rules. For more information, see Troubleshooting matchmaking rules using metrics and Testing rule sets with player traffic using metrics.

## Topics

### Getting match request metrics

Get rule-based match requests

Get match requests that use matchmaking rules.

Get classic match requests

Get match requests that don’t use matchmaking rules.

### Getting rule results and errors

Get Boolean rule results

Get the results of a specific matchmaking rule that returns Boolean values.

Get numeric rule results

Get the results of a specific matchmaking rule that returns numeric values.

Get matchmaking rule errors

Get errors that occur for a specific matchmaking rule.

### Getting queue information

Get queue size

Get the time that match requests are in a specific queue.

Get experimental queue size

Get the number of match requests that the queue processes using its experimental rule set.

Get match request time in queue

Get the match requests that a specific queue processes.

Get experimental match request time in queue

Get the match requests that a specific queue processes using its experimental rule set.

Get queue session information

Get session information on a queue.

### Objects

object GameCenterMatchmakingAppRequestsV1MetricResponse

The response body for fetching a match request.

object GameCenterMatchmakingBooleanRuleResultsV1MetricResponse

The response body for fetching the results of applying Boolean rules.

object GameCenterMatchmakingNumberRuleResultsV1MetricResponse

The response body for fetching the results of applying numeric rules.

object GameCenterMatchmakingRuleErrorsV1MetricResponse

The response body for fetching the rule errors.

object GameCenterMatchmakingQueueSizesV1MetricResponse

The response body for fetching the queue sizes.

object GameCenterMatchmakingQueueRequestsV1MetricResponse

The response body for match requests in a queue.

object GameCenterMatchmakingSessionsV1MetricResponse

The response body for information about a successful matchmaking session.

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

Testing

Test matchmaking rules using sample data.

