

- GameKit
- GKMatchmakerViewControllerDelegate
-  matchmakerViewController(\_:didFindPlayers:) Deprecated

Instance Method

# matchmakerViewController(\_:didFindPlayers:)

Called when a hosted match is found.

iOS 4.1–8.0DeprecatediPadOS 4.1–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func matchmakerViewController(
    _ viewController: GKMatchmakerViewController,
    didFindPlayers playerIDs: [String]
)
```

## Parameters 

`viewController`  

The view controller that performed the matchmaking.

`playerIDs`  

An array of `NSString` objects containing player identifier for the matched players.

## Discussion

This method is called when the view controller’s `hosted` property is true. Although optional in the protocol, if your game attaches a delegate to the view controller for a hosted match, the view controller expects your game to provide an implementation of this method.

The view controller returns the list of players to your game by calling this method. Your game is responsible for connecting these players to your own server and then using that server to relay messages between the players.

## See Also

### Related Documentation

func matchmakerViewController(GKMatchmakerViewController, didFind: GKMatch)

Handles when the view controller finds players for a peer-to-peer match.

### Deprecated Methods

func matchmakerViewController(GKMatchmakerViewController, didReceiveAcceptFromHostedPlayer: String)

Called when a player in a hosted match accepts the invitation.

Deprecated

