

- GameKit
- GKGameSessionEventListener
-  session(\_:didAdd:) Deprecated

Instance Method

# session(\_:didAdd:)

Tells the listener a new player has been added to a game session.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func session(
    _ session: GKGameSession,
    didAdd player: GKCloudPlayer
)
```

## Parameters 

`session`  

The game session that added a player.

`player`  

The player that was added to the session.

## See Also

### Changing Player Status

func session(GKGameSession, didRemove: GKCloudPlayer)

Tells the listener a player left a game session.

Deprecated

func session(GKGameSession, player: GKCloudPlayer, didChange: GKConnectionState)

Tells the listener a player’s connection state has changed.

Deprecated

enum GKConnectionState

Possible connection states for a player

