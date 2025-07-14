

- GameKit
- GKMatchDelegate
-  match(\_:didReceive:forRecipient:fromRemotePlayer:) 

Instance Method

# match(\_:didReceive:forRecipient:fromRemotePlayer:)

Processes the data sent from one player to another.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
optional func match(
    _ match: GKMatch,
    didReceive data: Data,
    forRecipient recipient: GKPlayer,
    fromRemotePlayer player: GKPlayer
)
```

## Parameters 

`match`  

The match associated with the data.

`data`  

The data sent by the player.

`recipient`  

The player who receives the data.

`player`  

The player who sends the data.

## Discussion

Your game defines its own format for data packets it transmits and receives over the network.

Important

You need to treat data you receive from other players as *untrusted* data. Be sure to validate the data you receive from the match and write your code carefully to avoid security vulnerabilities.

## See Also

### Receiving Data from Other Players

func match(GKMatch, didReceive: Data, fromRemotePlayer: GKPlayer)

Processes the data sent from another player to the local player.

