

- TabletopKit
- TabletopGame
- TabletopGame.MultiplayerDelegate
-  multiplayerSessionFailed(reason:) 

Instance Method

# multiplayerSessionFailed(reason:)

We failed to start or join a new multiplayer session or had to terminate a previously started multiplayer session.

visionOS 2.0+

``` source
func multiplayerSessionFailed(reason: any Error)
```

**Required**

## See Also

### Handling errors

func didRejectPlayer(PlayerIdentifier, reason: any Error)

A player that tried to join was rejected or a player that previously joined our game was ejected.

**Required**

