

- GameKit
- GKGameSessionEventListener
-  session(\_:player:didChange:) Deprecated

Instance Method

# session(\_:player:didChange:)

Tells the listener a player’s connection state has changed.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func session(
    _ session: GKGameSession,
    player: GKCloudPlayer,
    didChange newState: GKConnectionState
)
```

## Parameters 

`session`  

The game session affected by the connection state change.

`player`  

The player who’s connection state has changed.

`newState`  

The new connection state for the player.

## See Also

### Changing Player Status

func session(GKGameSession, didAdd: GKCloudPlayer)

Tells the listener a new player has been added to a game session.

Deprecated

func session(GKGameSession, didRemove: GKCloudPlayer)

Tells the listener a player left a game session.

Deprecated

enum GKConnectionState

Possible connection states for a player

