

- GameKit
- GKGameSessionEventListener
-  session(\_:didReceive:from:) Deprecated

Instance Method

# session(\_:didReceive:from:)

Tells the listener the player received data from another player.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func session(
    _ session: GKGameSession,
    didReceive data: Data,
    from player: GKCloudPlayer
)
```

## Parameters 

`session`  

The game session the sending player is associated with.

`data`  

The data sent by the player.

`player`  

The player sending data to all other connected players in the game session.

## Discussion

This event fires after the send(_:with:completionHandler:) method has been called. All connected players except the calling player are notified.

## See Also

### Transferring Data

func session(GKGameSession, didReceiveMessage: String, with: Data, from: GKCloudPlayer)

Tells the listener a player has received a message from another player.

Deprecated

func session(GKGameSession, player: GKCloudPlayer, didSave: Data)

Tells the listener data was saved by a player.

Deprecated

