

- GameKit
- GKMatch
-  chooseBestHostingPlayer(completionHandler:) 

Instance Method

# chooseBestHostingPlayer(completionHandler:)

Determines the best player in the game to act as the server for a client-server topology.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func chooseBestHostingPlayer(completionHandler: @escaping (GKPlayer?) -> Void)
```

``` source
func chooseBestHostingPlayer() async -> GKPlayer?
```

## Parameters 

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameter:

`player`  
The player with the best estimated network performance, or `nil` if GameKit couldn’t determine the best host.

## Mentioned in 

Exchanging data between players in real-time games

## Discussion

This method estimates which player has the best network connection using a variety of metrics such as bandwidth, latency, and network reliability. Use this method to choose the player that acts as the server when you implement a client-server topology on top of the match’s peer-to-peer connection.

## See Also

### Sending data to other players

func send(Data, to: [GKPlayer], dataMode: GKMatch.SendDataMode) throws

Transmits data to one or more players connected to the match.

func sendData(toAllPlayers: Data, with: GKMatch.SendDataMode) throws

Transmits data to all players connected to the match.

enum SendDataMode

The mechanism used to transmit data to other players.

