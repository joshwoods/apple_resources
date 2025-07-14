

- GameKit
- GKMatch
-  send(\_:to:dataMode:) 

Instance Method

# send(\_:to:dataMode:)

Transmits data to one or more players connected to the match.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func send(
    _ data: Data,
    to players: [GKPlayer],
    dataMode mode: GKMatch.SendDataMode
) throws
```

## Parameters 

`data`  

The bytes to send.

`players`  

The players who receive the data.

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

func sendData(toAllPlayers: Data, with: GKMatch.SendDataMode) throws

Transmits data to all players connected to the match.

enum SendDataMode

The mechanism used to transmit data to other players.

