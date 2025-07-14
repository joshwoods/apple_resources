

- GameKit
- GKMatchmakerViewControllerDelegate
-  matchmakerViewController(\_:hostedPlayerDidAccept:) 

Instance Method

# matchmakerViewController(\_:hostedPlayerDidAccept:)

Handles when a player in a hosted match accepts the invitation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func matchmakerViewController(
    _ viewController: GKMatchmakerViewController,
    hostedPlayerDidAccept player: GKPlayer
)
```

## Parameters 

`viewController`  

The view controller that performs the matchmaking.

`player`  

The player that accepts the invitation to join the match.

## Discussion

After a player accepts an invitation, connect the player to your server. Once the connection is established, your game needs to call the view controller’s setHostedPlayer(_:didConnect:) method to update the player’s connection status.

