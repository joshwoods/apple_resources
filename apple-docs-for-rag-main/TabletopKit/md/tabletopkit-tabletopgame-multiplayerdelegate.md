

- TabletopKit
- TabletopGame
-  multiplayerDelegate 

Instance Property

# multiplayerDelegate

visionOS 2.0+

``` source
weak var multiplayerDelegate: (any TabletopGame.MultiplayerDelegate)? { get set }
```

## See Also

### Supporting multiple players

func attachNetworkCoordinator(some TabletopNetworkSessionCoordinator)

func detachNetworkCoordinator()

protocol MultiplayerDelegate

An object that handles players joining multiplayer games.

