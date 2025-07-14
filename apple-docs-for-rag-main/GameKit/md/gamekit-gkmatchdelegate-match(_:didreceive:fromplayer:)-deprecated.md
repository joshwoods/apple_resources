

- GameKit
- GKMatchDelegate
-  match(\_:didReceive:fromPlayer:) Deprecated

Instance Method

# match(\_:didReceive:fromPlayer:)

Handles when a player receives data in a match.

iOS 4.1–8.0DeprecatediPadOS 4.1–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func match(
    _ match: GKMatch,
    didReceive data: Data,
    fromPlayer playerID: String
)
```

## Parameters 

`match`  

The match that received the data.

`data`  

The bytes sent by the player.

`playerID`  

The string identifier for the player that sent the data.

## Discussion

You define your own format for data packets that you transmit and receive over the network.

Important

You need to treat data you receive from other players as *untrusted* data. Be sure to validate the data you receive from the match and write your code carefully to avoid security vulnerabilities.

## See Also

### Deprecated Methods and Properties

func match(GKMatch, player: String, didChange: GKPlayerConnectionState)

Handles when a player connects or disconnects from a match.

Deprecated

func match(GKMatch, shouldReinvitePlayer: String) -> Bool

Handles when a player disconnects from a two-player match.

Deprecated

