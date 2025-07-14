

- GameKit
- GKMatchmakerViewControllerDelegate
-  matchmakerViewController(\_:didFind:) 

Instance Method

# matchmakerViewController(\_:didFind:)

Handles when the view controller finds players for a peer-to-peer match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
optional func matchmakerViewController(
    _ viewController: GKMatchmakerViewController,
    didFind match: GKMatch
)
```

## Parameters 

`viewController`  

The view controller that finds players for the match.

`match`  

The match that the players join.

## Mentioned in 

Finding multiple players for a game

Finding players using matchmaking rules

Exchanging data between players in real-time games

Finding players with similar skill levels

Assigning players to teams using rules

## Discussion

When all the players accept their invitations to a match, GameKit invokes this method in the app instances for all players in the match, including the local player who initiates the match. This method needs to dismiss the view controller and start the game. Use the match object passed to this method to get the players and communicate between them during the game.

Although this method appears optional in the protocol, if you set the view controller’s delegate for a peer-to-peer match, GameKit expects the delegate to implement this method. If the view controller’s isHosted property is true, GameKit instead invokes the matchmakerViewController(_:didFindHostedPlayers:) method.

## See Also

### Starting matches

func matchmakerViewController(GKMatchmakerViewController, didFindHostedPlayers: [GKPlayer])

Handles when the view controller finds all requested players for a hosted match.

