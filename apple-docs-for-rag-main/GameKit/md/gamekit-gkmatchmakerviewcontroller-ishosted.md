

- GameKit
- GKMatchmakerViewController
-  isHosted 

Instance Property

# isHosted

A Boolean value that indicates whether the match is hosted or peer-to-peer.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var isHosted: Bool { get set }
```

## Discussion

The value of this property determines which delegate methods GameKit calls when players are found.

If you host your own game, set this property to `true,` and then GameKit calls the matchmakerViewController(_:didFindHostedPlayers:) delegate method when it finds players. You must provide a server that hosts the players in the match.

Otherwise, set this property to false, and then GameKit calls the matchmakerViewController(_:didFind:) delegate method when it finds players.

## See Also

### Hosting matches

func setHostedPlayer(GKPlayer, didConnect: Bool)

Updates the connection status of a player in a hosted game.

