

- GameKit
- GKMatchDelegate
-  match(\_:didReceive:fromRemotePlayer:) 

Instance Method

# match(\_:didReceive:fromRemotePlayer:)

Processes the data sent from another player to the local player.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func match(
    _ match: GKMatch,
    didReceive data: Data,
    fromRemotePlayer player: GKPlayer
)
```

## Parameters 

`match`  

The match associated with the data.

`data`  

The data sent by the player.

`player`  

The player who sends the data.

## Mentioned in 

Exchanging data between players in real-time games

## Discussion

Your game defines its own format for data packets it transmits and receives over the network.

Important

You need to treat data you receive from other players as *untrusted* data. Be sure to validate the data you receive from the match and write your code carefully to avoid security vulnerabilities.

## See Also

### Receiving Data from Other Players

func match(GKMatch, didReceive: Data, forRecipient: GKPlayer, fromRemotePlayer: GKPlayer)

Processes the data sent from one player to another.

