

- GameKit
- GKMatchmakerViewController
-  setHostedPlayer(\_:connected:) Deprecated

Instance Method

# setHostedPlayer(\_:connected:)

Updates a player’s status on the view to show that the player has connected or disconnected from your server.

iOS 5.0–8.0DeprecatediPadOS 5.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func setHostedPlayer(
    _ playerID: String,
    connected: Bool
)
```

Deprecated

Use the setHostedPlayer(_:didConnect:) method instead.

## Parameters 

`playerID`  

The identifier string for a player that connected to the external server.

`connected`  

A Boolean value that states whether the player is connected to the hosted match.

## Discussion

When setting up a hosted match, each device needs to create a matchmaker view controller and display it to the player. Then, when a new player connects to your server, your server needs to notify all participating devices already connected to your server. Each participating device then calls this method to update that player’s status in the matchmaking interface. Similarly, if a player disconnects from the server, your server informs each device so the devices can update their user interface.

## See Also

### Deprecated

func setHostedPlayerReady(String)

Informs the controller that a player has joined a hosted match.

Deprecated

var defaultInvitationMessage: String?

The default invitation message sent to a player.

Deprecated

