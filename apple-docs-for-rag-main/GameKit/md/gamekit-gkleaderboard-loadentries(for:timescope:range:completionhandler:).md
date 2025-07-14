

- GameKit
- GKLeaderboard
-  loadEntries(for:timeScope:range:completionHandler:) 

Instance Method

# loadEntries(for:timeScope:range:completionHandler:)

Returns the scores for the local player and other players for the specified type of player, time period, and ranks.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func loadEntries(
    for playerScope: GKLeaderboard.PlayerScope,
    timeScope: GKLeaderboard.TimeScope,
    range: NSRange,
    completionHandler: @escaping (GKLeaderboard.Entry?, [GKLeaderboard.Entry]?, Int, (any Error)?) -> Void
)
```

``` source
func loadEntries(
    for playerScope: GKLeaderboard.PlayerScope,
    timeScope: GKLeaderboard.TimeScope,
    range: NSRange
) async throws -> (GKLeaderboard.Entry?, [GKLeaderboard.Entry], Int)
```

## Parameters 

`playerScope`  

Specifies whether to get scores from friends or all players.

`timeScope`  

Specifies the time period for the scores. This parameter is applicable to nonrecurring leaderboards only. For recurring leaderboards, pass GKLeaderboard.TimeScope.allTime for this parameter.

`range`  

Specifies the range of ranks to use for getting the scores. The difference between the minimum rank and maximum rank must not exceed `100`.

`completionHandler`  

A block that GameKit calls when this method completes the request.

The block receives the following parameters:

localPlayerEntry  
The score for the local player, or `nil` if the player has no score.

entries  
The scores this method loads that match the `playerScope`, `timeScope`, and `range` parameters, including the local player’s score if it exists.

totalPlayerCount  
The total number of players whose scores match the `playerScope` and `timeScope` parameters, but not the `range` parameter.

error  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Encourage progress and competition with leaderboards

## Discussion

GameKit uses the following algorithm to fetch GKLeaderboard scores:

1.  Begins with the set of all possible scores for the leaderboard.

2.  Discards any scores that don’t match the `playerScope` and `timeScope` properties.

3.  For each player, keeps the best score that player earns and discards the rest.

4.  Sorts the scores from best to worst.

5.  Uses the range property to determine which scores return.

## See Also

### Loading Scores

func loadEntries(for: [GKPlayer], timeScope: GKLeaderboard.TimeScope, completionHandler: (GKLeaderboard.Entry?, [GKLeaderboard.Entry]?, (any Error)?) -> Void)

Returns the scores for the local player and other players for the specified time period.

enum PlayerScope

Specifies the type of players for filtering data.

enum TimeScope

Specifies the time period for filtering data.

class Entry

Information about a single score by a player on a leaderboard.

