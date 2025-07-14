

- GameKit
- GKTurnBasedMatch
-  endMatchInTurn(withMatch:leaderboardScores:achievements:completionHandler:) 

Instance Method

# endMatchInTurn(withMatch:leaderboardScores:achievements:completionHandler:)

Ends the match while submitting scores and achievements for all of the participants.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func endMatchInTurn(
    withMatch matchData: Data,
    leaderboardScores scores: [GKLeaderboardScore],
    achievements: [Any],
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func endMatchInTurn(
    withMatch matchData: Data,
    leaderboardScores scores: [GKLeaderboardScore],
    achievements: [Any]
) async throws
```

## Parameters 

`matchData`  

Your game-specific data representing the match state. For example, include information needed for the next participant to take their turn in this object. Don’t pass `nil` as this parameter.

`scores`  

The final scores that each participant earns in the match. The scores can be for different leaderboards.

`achievements`  

The achievements that each participant acquires in the match.

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameter:

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

Invoke this method only when the local player is the current participant. Also, set the matchOutcome property for each participant in the match’s participants property to a value other than GKTurnBasedMatch.Outcome.none before invoking this method.

To receive turn-based events that this method generates, register a listener that conforms to the GKTurnBasedEventListener protocol with the local player. See Starting turn-based matches and passing turns between players.

## See Also

### Ending a Match

func endMatchInTurn(withMatch: Data, completionHandler: (((any Error)?) -> Void)?)

Ends the match.

