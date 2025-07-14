

- GameKit
- GKMatchmakerViewController
-  setHostedPlayerReady(\_:) Deprecated

Instance Method

# setHostedPlayerReady(\_:)

Informs the controller that a player has joined a hosted match.

visionOS 1.0–1.0Deprecated

``` source
@MainActor
func setHostedPlayerReady(_ playerID: String)
```

Deprecated

Use the setHostedPlayer(_:connected:) method instead.

## Parameters 

`playerID`  

The identifier string for a player that connected to the external server.

## Discussion

In a hosted match, when a new player connects to the server, your server needs to inform all participating devices connected to the match. Each participating device must separately call this method to update its matchmaking user interface.

## See Also

### Deprecated

func setHostedPlayer(String, connected: Bool)

Updates a player’s status on the view to show that the player has connected or disconnected from your server.

Deprecated

var defaultInvitationMessage: String?

The default invitation message sent to a player.

Deprecated

