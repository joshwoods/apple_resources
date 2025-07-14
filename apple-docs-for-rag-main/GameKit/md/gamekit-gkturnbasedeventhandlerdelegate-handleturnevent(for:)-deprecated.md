

- GameKit
- GKTurnBasedEventHandlerDelegate
-  handleTurnEvent(for:) Deprecated

Instance Method

# handleTurnEvent(for:)

Sent to the delegate when it is the local player’s turn to act in a turn-based match.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
optional func handleTurnEvent(for match: GKTurnBasedMatch)
```

Deprecated

Implement handleTurnEvent(for:didBecomeActive:) instead.

## Parameters 

`match`  

A match object containing the current state of the match.

## Discussion

When your delegate receives this message, the player has accepted a push notification for a match already in progress. Your game should end whatever task it was performing and switch to the match information provided by the match object.

## See Also

### Receiving Turn-based Events

func handleInvite(fromGameCenter: [String])

Sent to the delegate when the local player receives an invitation to join a new turn-based match.

**Required**

Deprecated

func handleTurnEvent(for: GKTurnBasedMatch, didBecomeActive: Bool)

Sent to the delegate when it is the local player’s turn to act in a turn-based match.

**Required**

Deprecated

func handleMatchEnded(GKTurnBasedMatch)

Sent to the delegate when a match the local player is participating in has ended.

Deprecated

