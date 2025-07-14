

- GameKit
- GKGameSessionEventListener
-  session(\_:didRemove:) Deprecated

Instance Method

# session(\_:didRemove:)

Tells the listener a player left a game session.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func session(
    _ session: GKGameSession,
    didRemove player: GKCloudPlayer
)
```

## Parameters 

`session`  

The game session the player left.

`player`  

The player that left the game session.

## See Also

### Changing Player Status

func session(GKGameSession, didAdd: GKCloudPlayer)

Tells the listener a new player has been added to a game session.

Deprecated

func session(GKGameSession, player: GKCloudPlayer, didChange: GKConnectionState)

Tells the listener a player’s connection state has changed.

Deprecated

enum GKConnectionState

Possible connection states for a player

