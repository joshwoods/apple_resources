

- GameKit
- GKTurnBasedEventHandlerDelegate
-  handleMatchEnded(\_:) Deprecated

Instance Method

# handleMatchEnded(\_:)

Sent to the delegate when a match the local player is participating in has ended.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
optional func handleMatchEnded(_ match: GKTurnBasedMatch)
```

## Parameters 

`match`  

The match that just ended.

## Discussion

When your delegate receives this message, it should display the match’s final results to the player and allow the player the option of saving or removing the match data from Game Center.

## See Also

### Receiving Turn-based Events

func handleInvite(fromGameCenter: [String])

Sent to the delegate when the local player receives an invitation to join a new turn-based match.

**Required**

Deprecated

func handleTurnEvent(for: GKTurnBasedMatch)

Sent to the delegate when it is the local player’s turn to act in a turn-based match.

Deprecated

func handleTurnEvent(for: GKTurnBasedMatch, didBecomeActive: Bool)

Sent to the delegate when it is the local player’s turn to act in a turn-based match.

**Required**

Deprecated

