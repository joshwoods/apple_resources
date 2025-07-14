

- GameKit
-  GKTransportType 

Enumeration

# GKTransportType

The mechanism used to send messages to other players in a game session.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
enum GKTransportType
```

## Topics

### Constants

case reliable

The data is sent continuously until it is successfully received by the intended recipients or the connection times out.

case unreliable

The data is sent once and is not sent again if a transmission error occurs.

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

### Connecting Players for Real-Time Communication

func setConnectionState(GKConnectionState, completionHandler: ((any Error)?) -> Void)

Sets the connection state for the player.

Deprecated

func players(with: GKConnectionState) -> [GKCloudPlayer]

Retrieves a list of players with the specified connection state.

Deprecated

func send(Data, with: GKTransportType, completionHandler: ((any Error)?) -> Void)

Sends the indicated data to all connected players.

Deprecated

