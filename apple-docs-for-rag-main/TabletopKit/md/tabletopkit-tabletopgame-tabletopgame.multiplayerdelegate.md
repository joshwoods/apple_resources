

- TabletopKit
- TabletopGame
-  TabletopGame.MultiplayerDelegate 

Protocol

# TabletopGame.MultiplayerDelegate

An object that handles players joining multiplayer games.

visionOS 2.0+

``` source
protocol MultiplayerDelegate : AnyObject
```

## Topics

### Joining games

func joinAccepted()

We tried to join a game and got accepted

**Required**

func playerJoined(PlayerIdentifier)

A player joined our multiplayer session

**Required**

### Handling errors

func didRejectPlayer(PlayerIdentifier, reason: any Error)

A player that tried to join was rejected or a player that previously joined our game was ejected.

**Required**

func multiplayerSessionFailed(reason: any Error)

We failed to start or join a new multiplayer session or had to terminate a previously started multiplayer session.

**Required**

## See Also

### Supporting multiple players

func attachNetworkCoordinator(some TabletopNetworkSessionCoordinator)

func detachNetworkCoordinator()

var multiplayerDelegate: (any TabletopGame.MultiplayerDelegate)?

