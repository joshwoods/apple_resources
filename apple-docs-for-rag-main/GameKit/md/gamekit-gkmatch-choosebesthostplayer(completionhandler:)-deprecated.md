

- GameKit
- GKMatch
-  chooseBestHostPlayer(completionHandler:) Deprecated

Instance Method

# chooseBestHostPlayer(completionHandler:)

Determines the best player in the game to act as the server for a client-server match.

iOS 6.0–8.0DeprecatediPadOS 6.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.10DeprecatedvisionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, visionOS**

``` source
func chooseBestHostPlayer(completionHandler: @escaping (String?) -> Void)
```

**Mac Catalyst, visionOS**

``` source
func chooseBestHostPlayer() async -> String?
```

Deprecated

Use the chooseBestHostingPlayer(completionHandler:) method instead.

## Parameters 

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameter:

`playerID`  
The player identifier for the player with the best estimated network performance, or `nil` if GameKit couldn’t find a best host player.

## Discussion

Calling this method causes GameKit to attempt to estimate which player has the best overall network connection using a variety of metrics such as bandwidth, latency, and network reliability. Typically, you call this method when your game implements a client-server model on top of the match’s peer-to-peer connection.

## See Also

### Deprecated Methods and Properties

var playerIDs: [String]?

The player identifiers for remote players in the match.

Deprecated

func send(Data, toPlayers: [String], with: GKMatch.SendDataMode) throws

Transmits data to a list of connected players.

Deprecated

