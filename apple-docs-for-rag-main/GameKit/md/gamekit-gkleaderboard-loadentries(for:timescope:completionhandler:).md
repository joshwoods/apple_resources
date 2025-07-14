

- GameKit
- GKLeaderboard
-  loadEntries(for:timeScope:completionHandler:) 

Instance Method

# loadEntries(for:timeScope:completionHandler:)

Returns the scores for the local player and other players for the specified time period.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func loadEntries(
    for players: [GKPlayer],
    timeScope: GKLeaderboard.TimeScope,
    completionHandler: @escaping (GKLeaderboard.Entry?, [GKLeaderboard.Entry]?, (any Error)?) -> Void
)
```

``` source
func loadEntries(
    for players: [GKPlayer],
    timeScope: GKLeaderboard.TimeScope
) async throws -> (GKLeaderboard.Entry?, [GKLeaderboard.Entry])
```

## Parameters 

`players`  

The players whose scores this method returns.

`timeScope`  

Specifies the time period for the scores. This parameter is applicable to nonrecurring leaderboards only. For recurring leaderboards, pass GKLeaderboard.TimeScope.allTime for this parameter.

`completionHandler`  

A block that GameKit calls when this method loads the scores.

The block receives the following parameters:

localPlayerEntry  
The score for the local player, or `nil` if the player has no score.

entries  
The scores for the players during the specified time period, including the local player’s score if it exists.

error  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Connecting players with their friends in your game

## See Also

### Loading Scores

func loadEntries(for: GKLeaderboard.PlayerScope, timeScope: GKLeaderboard.TimeScope, range: NSRange, completionHandler: (GKLeaderboard.Entry?, [GKLeaderboard.Entry]?, Int, (any Error)?) -> Void)

Returns the scores for the local player and other players for the specified type of player, time period, and ranks.

enum PlayerScope

Specifies the type of players for filtering data.

enum TimeScope

Specifies the time period for filtering data.

class Entry

Information about a single score by a player on a leaderboard.

