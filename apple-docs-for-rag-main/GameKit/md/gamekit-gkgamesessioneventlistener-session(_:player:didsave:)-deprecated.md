

- GameKit
- GKGameSessionEventListener
-  session(\_:player:didSave:) Deprecated

Instance Method

# session(\_:player:didSave:)

Tells the listener data was saved by a player.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func session(
    _ session: GKGameSession,
    player: GKCloudPlayer,
    didSave data: Data
)
```

## Parameters 

`session`  

The game session data was saved to.

`player`  

The player that just saved data.

`data`  

The data that was saved.

## See Also

### Transferring Data

func session(GKGameSession, didReceive: Data, from: GKCloudPlayer)

Tells the listener the player received data from another player.

Deprecated

func session(GKGameSession, didReceiveMessage: String, with: Data, from: GKCloudPlayer)

Tells the listener a player has received a message from another player.

Deprecated

