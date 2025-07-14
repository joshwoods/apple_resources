

- GameKit
- GKTurnBasedEventHandlerDelegate
-  handleTurnEvent(for:didBecomeActive:) Deprecated

Instance Method

# handleTurnEvent(for:didBecomeActive:)

Sent to the delegate when it is the local player’s turn to act in a turn-based match.

macOS 10.9–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
func handleTurnEvent(
    for match: GKTurnBasedMatch,
    didBecomeActive: Bool
)
```

**Required**

## Parameters 

`match`  

A match object containing the current state of the match.

`didBecomeActive`  

true if the game was launched or brought to the foreground to handle the event.

## Discussion

When your delegate receives this message, the player has accepted a push notification for a match already in progress. Your game should end whatever task it was performing and switch to the match information provided by the match object.

## See Also

### Receiving Turn-based Events

func handleInvite(fromGameCenter: [String])

Sent to the delegate when the local player receives an invitation to join a new turn-based match.

**Required**

Deprecated

func handleTurnEvent(for: GKTurnBasedMatch)

Sent to the delegate when it is the local player’s turn to act in a turn-based match.

Deprecated

func handleMatchEnded(GKTurnBasedMatch)

Sent to the delegate when a match the local player is participating in has ended.

Deprecated

