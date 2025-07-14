

- GameKit
- GKMatchmakerViewControllerDelegate
-  matchmakerViewController(\_:didFindHostedPlayers:) 

Instance Method

# matchmakerViewController(\_:didFindHostedPlayers:)

Handles when the view controller finds all requested players for a hosted match.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func matchmakerViewController(
    _ viewController: GKMatchmakerViewController,
    didFindHostedPlayers players: [GKPlayer]
)
```

## Parameters 

`viewController`  

The view controller that finds players for the match.

`players`  

The players who accept an invitation to this match.

## Discussion

When all the players accept their invitations to a match, GameKit invokes this method in the app instances for all players in the game, including the local player who initiates the invitations. This method needs to dismiss the view controller and start the game. Your game needs to connect the players to your own server and then use that server to relay messages between the players.

Although this method appears optional in the protocol, if you set the view controller’s delegate for a hosted match, GameKit expects the delegate to implement this method. If the view controller’s isHosted property is false, GameKit instead invokes the matchmakerViewController(_:didFind:) method.

## See Also

### Starting matches

func matchmakerViewController(GKMatchmakerViewController, didFind: GKMatch)

Handles when the view controller finds players for a peer-to-peer match.

