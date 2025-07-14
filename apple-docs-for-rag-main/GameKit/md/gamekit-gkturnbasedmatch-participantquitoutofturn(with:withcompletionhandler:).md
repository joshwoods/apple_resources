

- GameKit
- GKTurnBasedMatch
-  participantQuitOutOfTurn(with:withCompletionHandler:) 

Instance Method

# participantQuitOutOfTurn(with:withCompletionHandler:)

Forfeits the match on behalf of the local player when it’s not their turn.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func participantQuitOutOfTurn(
    with matchOutcome: GKTurnBasedMatch.Outcome,
    withCompletionHandler completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func participantQuitOutOfTurn(with matchOutcome: GKTurnBasedMatch.Outcome) async throws
```

## Parameters 

`matchOutcome`  

The outcome of the local player who forfeits the match. Don’t pass `nil` as this parameter.

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameter:

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

Invoke this method to forfeit a match when the local player isn’t the current participant. To receive turn-based events that this method generates, register a listener that conforms to the GKTurnBasedEventListener protocol with the local player. See Starting turn-based matches and passing turns between players.

## See Also

### Forfeiting a Match

func participantQuitInTurn(with: GKTurnBasedMatch.Outcome, nextParticipants: [GKTurnBasedParticipant], turnTimeout: TimeInterval, match: Data, completionHandler: (((any Error)?) -> Void)?)

Forfeits the match on behalf of the local player when it’s their turn.

enum Outcome

The state of a participant when they forfeit a match or when a match ends.

