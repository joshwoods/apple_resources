

- GameKit
- GKTurnBasedEventHandlerDelegate
-  handleInvite(fromGameCenter:) Deprecated

Instance Method

# handleInvite(fromGameCenter:)

Sent to the delegate when the local player receives an invitation to join a new turn-based match.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
func handleInvite(fromGameCenter playersToInvite: [String])
```

**Required**

## Parameters 

`playersToInvite`  

An array of `NSString` objects containing the player identifiers for the players to initially invite to the game.

## Discussion

When your delegate receives this message, your game should create a new GKMatchRequest object and assign the `playersToInvite` parameter to the match request’s playersToInvite property. Then, your game can either call the GKTurnBasedMatch class method find(for:withCompletionHandler:) to find a match programmatically or it can use the request to instantiate a new GKTurnBasedMatchmakerViewController object to show a user interface to the player.

## See Also

### Receiving Turn-based Events

func handleTurnEvent(for: GKTurnBasedMatch)

Sent to the delegate when it is the local player’s turn to act in a turn-based match.

Deprecated

func handleTurnEvent(for: GKTurnBasedMatch, didBecomeActive: Bool)

Sent to the delegate when it is the local player’s turn to act in a turn-based match.

**Required**

Deprecated

func handleMatchEnded(GKTurnBasedMatch)

Sent to the delegate when a match the local player is participating in has ended.

Deprecated

