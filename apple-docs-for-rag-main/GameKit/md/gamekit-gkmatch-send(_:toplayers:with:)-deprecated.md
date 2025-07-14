

- GameKit
- GKMatch
-  send(\_:toPlayers:with:) Deprecated

Instance Method

# send(\_:toPlayers:with:)

Transmits data to a list of connected players.

iOS 4.1–8.0DeprecatediPadOS 4.1–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func send(
    _ data: Data,
    toPlayers playerIDs: [String],
    with mode: GKMatch.SendDataMode
) throws
```

Deprecated

Use the sendData(toAllPlayers:with:) method instead.

## Parameters 

`data`  

The bytes to send.

`playerIDs`  

The identifier strings for the list of players who should receive the data.

`mode`  

The mechanism used to send the data.

## Discussion

The match queues the data and transmits it when the network becomes available.

## See Also

### Deprecated Methods and Properties

func chooseBestHostPlayer(completionHandler: (String?) -> Void)

Determines the best player in the game to act as the server for a client-server match.

Deprecated

var playerIDs: [String]?

The player identifiers for remote players in the match.

Deprecated

