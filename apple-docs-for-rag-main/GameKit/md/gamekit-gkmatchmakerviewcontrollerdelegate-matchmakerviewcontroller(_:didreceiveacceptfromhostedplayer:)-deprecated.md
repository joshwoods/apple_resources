

- GameKit
- GKMatchmakerViewControllerDelegate
-  matchmakerViewController(\_:didReceiveAcceptFromHostedPlayer:) Deprecated

Instance Method

# matchmakerViewController(\_:didReceiveAcceptFromHostedPlayer:)

Called when a player in a hosted match accepts the invitation.

iOS 5.0–8.0DeprecatediPadOS 5.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func matchmakerViewController(
    _ viewController: GKMatchmakerViewController,
    didReceiveAcceptFromHostedPlayer playerID: String
)
```

## Parameters 

`viewController`  

The view controller that accepted the invitation.

`playerID`  

The identifier of the accepting player.

## Discussion

After a player accepts an invitation, that player’s device should connect to your server. Once the connection is established, your game should call the view controller’s setHostedPlayer(_:connected:) method to update the player’s connection status.

## See Also

### Deprecated Methods

func matchmakerViewController(GKMatchmakerViewController, didFindPlayers: [String])

Called when a hosted match is found.

Deprecated

