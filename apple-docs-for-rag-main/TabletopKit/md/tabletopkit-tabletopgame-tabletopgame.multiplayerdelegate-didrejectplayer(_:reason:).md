

- TabletopKit
- TabletopGame
- TabletopGame.MultiplayerDelegate
-  didRejectPlayer(\_:reason:) 

Instance Method

# didRejectPlayer(\_:reason:)

A player that tried to join was rejected or a player that previously joined our game was ejected.

visionOS 2.0+

``` source
func didRejectPlayer(
    _ playerID: PlayerIdentifier,
    reason: any Error
)
```

**Required**

## See Also

### Handling errors

func multiplayerSessionFailed(reason: any Error)

We failed to start or join a new multiplayer session or had to terminate a previously started multiplayer session.

**Required**

