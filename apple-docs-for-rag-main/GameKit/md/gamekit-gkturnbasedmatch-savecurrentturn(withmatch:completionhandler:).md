

- GameKit
- GKTurnBasedMatch
-  saveCurrentTurn(withMatch:completionHandler:) 

Instance Method

# saveCurrentTurn(withMatch:completionHandler:)

Saves your match data in Game Center without ending the turn.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func saveCurrentTurn(
    withMatch matchData: Data,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func saveCurrentTurn(withMatch matchData: Data) async throws
```

## Parameters 

`matchData`  

Your game-specific data representing the match state. For example, include the current participant’s activity while taking their turn in this object. Don’t pass `nil` as this parameter.

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameter:

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

Invoke this method only when the local player is the current participant. To receive turn-based events that this method generates, register a listener that conforms to the GKTurnBasedEventListener protocol with the local player. See Starting turn-based matches and passing turns between players.

## See Also

### Ending Turns and Saving Data

func endTurn(withNextParticipants: [GKTurnBasedParticipant], turnTimeout: TimeInterval, match: Data, completionHandler: (((any Error)?) -> Void)?)

Passes the turn from the current participant to the next participant.

Turn Timeouts

A timeout for a player to take their turn.

