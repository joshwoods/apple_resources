

- GameKit
- GKMatch
-  sendData(toAllPlayers:with:) 

Instance Method

# sendData(toAllPlayers:with:)

Transmits data to all players connected to the match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func sendData(
    toAllPlayers data: Data,
    with mode: GKMatch.SendDataMode
) throws
```

## Parameters 

`data`  

The bytes to send.

`mode`  

The mechanism used to send the data.

## Mentioned in 

Exchanging data between players in real-time games

## Discussion

The match queues the data and transmits it when the network becomes available.

## See Also

### Sending data to other players

func chooseBestHostingPlayer(completionHandler: (GKPlayer?) -> Void)

Determines the best player in the game to act as the server for a client-server topology.

func send(Data, to: [GKPlayer], dataMode: GKMatch.SendDataMode) throws

Transmits data to one or more players connected to the match.

enum SendDataMode

The mechanism used to transmit data to other players.

