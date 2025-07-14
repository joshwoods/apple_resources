

- GameKit
- GKGameSessionEventListener
-  session(\_:didReceiveMessage:with:from:) Deprecated

Instance Method

# session(\_:didReceiveMessage:with:from:)

Tells the listener a player has received a message from another player.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func session(
    _ session: GKGameSession,
    didReceiveMessage message: String,
    with data: Data,
    from player: GKCloudPlayer
)
```

## Parameters 

`session`  

The game session the sending player is associated with.

`message`  

A `String` containing the message sent to other players.

`data`  

Any data associated with the message. The value of this parameter can be `nil`.

`player`  

The player who sent the message.

## Discussion

This event fires after the sendMessage(withLocalizedFormatKey:arguments:data:to:badgePlayers:completionHandler:) method has been called. Only players contained in the `players` argument of the sendMessage(withLocalizedFormatKey:arguments:data:to:badgePlayers:completionHandler:) method are notified.

## See Also

### Transferring Data

func session(GKGameSession, didReceive: Data, from: GKCloudPlayer)

Tells the listener the player received data from another player.

Deprecated

func session(GKGameSession, player: GKCloudPlayer, didSave: Data)

Tells the listener data was saved by a player.

Deprecated

