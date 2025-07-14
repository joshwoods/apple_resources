

- GameKit
- GKTurnBasedMatch
-  endMatchInTurn(withMatch:completionHandler:) 

Instance Method

# endMatchInTurn(withMatch:completionHandler:)

Ends the match.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func endMatchInTurn(
    withMatch matchData: Data,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func endMatchInTurn(withMatch matchData: Data) async throws
```

## Parameters 

`matchData`  

Your game-specific data representing the match state. For example, include information needed for the next participant to take their turn in this object. Don’t pass `nil` as this parameter.

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

func endMatchInTurn(withMatch: Data, leaderboardScores: [GKLeaderboardScore], achievements: [Any], completionHandler: ((any Error)?) -> Void)

Ends the match while submitting scores and achievements for all of the participants.

