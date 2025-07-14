

- GameKit
-  GKMatchType 

Enumeration

# GKMatchType

The kind of match managed by Game Center.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
enum GKMatchType
```

## Topics

### Types

case peerToPeer

A peer-to-peer match hosted by Game Center.

case hosted

A match hosted on your private server.

case turnBased

A turn-based match hosted by Game Center.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Restricting the number of players

class func maxPlayersAllowedForMatch(of: GKMatchType) -> Int

Returns the maximum number of players allowed in the match request for a given match type.

var minPlayers: Int

The minimum number of players that can join the match.

var maxPlayers: Int

The maximum number of players that can join the match.

var defaultNumberOfPlayers: Int

The default number of players for the match.

