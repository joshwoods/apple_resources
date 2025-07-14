

- GameKit
-  GKConnectionState 

Enumeration

# GKConnectionState

Possible connection states for a player

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
enum GKConnectionState
```

## Topics

### Constants

case connected

The player is connected to the game session.

case notConnected

The player is not connected to the game session.

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

### Changing Player Status

func session(GKGameSession, didAdd: GKCloudPlayer)

Tells the listener a new player has been added to a game session.

Deprecated

func session(GKGameSession, didRemove: GKCloudPlayer)

Tells the listener a player left a game session.

Deprecated

func session(GKGameSession, player: GKCloudPlayer, didChange: GKConnectionState)

Tells the listener a player’s connection state has changed.

Deprecated

