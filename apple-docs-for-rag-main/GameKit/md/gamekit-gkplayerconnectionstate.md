

- GameKit
-  GKPlayerConnectionState 

Enumeration

# GKPlayerConnectionState

The possible states of a connection to a match.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
enum GKPlayerConnectionState
```

## Topics

### States

case unknown

An undetermined state in which the player can’t receive data.

case connected

A state in which a player connects to the match and can receive data.

case disconnected

A state in which a player disconnects from the match and can’t receive data.

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

### Receiving State Notifications About Other Players

func match(GKMatch, player: GKPlayer, didChange: GKPlayerConnectionState)

Handles when players connect or disconnect from a match.

