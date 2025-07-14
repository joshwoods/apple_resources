

- GameKit
- GKMatchmakerViewController
-  defaultInvitationMessage Deprecated

Instance Property

# defaultInvitationMessage

The default invitation message sent to a player.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var defaultInvitationMessage: String? { get set }
```

Deprecated

Use the inviteMessage property instead.

## Discussion

Your game sets this property to change the default invitation text displayed when the local player creates a new invitation. The local player may edit the text before sending the invitation.

## See Also

### Deprecated

func setHostedPlayer(String, connected: Bool)

Updates a player’s status on the view to show that the player has connected or disconnected from your server.

Deprecated

func setHostedPlayerReady(String)

Informs the controller that a player has joined a hosted match.

Deprecated

