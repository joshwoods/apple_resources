

- GameKit
- GKMatch
-  GKMatch.SendDataMode 

Enumeration

# GKMatch.SendDataMode

The mechanism used to transmit data to other players.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
enum SendDataMode
```

## Topics

### Modes

case reliable

Sends data continuously until the recipients successfully receive it or the connection times out.

case unreliable

Sends data once even if an error occurs.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Sending data to other players

func chooseBestHostingPlayer(completionHandler: (GKPlayer?) -> Void)

Determines the best player in the game to act as the server for a client-server topology.

func send(Data, to: [GKPlayer], dataMode: GKMatch.SendDataMode) throws

Transmits data to one or more players connected to the match.

func sendData(toAllPlayers: Data, with: GKMatch.SendDataMode) throws

Transmits data to all players connected to the match.

