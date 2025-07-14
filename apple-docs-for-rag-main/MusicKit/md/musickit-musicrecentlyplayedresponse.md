

- MusicKit
-  MusicRecentlyPlayedResponse 

Structure

# MusicRecentlyPlayedResponse

An object that contains items the user has recently played.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicRecentlyPlayedResponse where MusicItemType : MusicRecentlyPlayedRequestable
```

## Topics

### Instance Properties

let items: MusicItemCollection&lt;MusicItemType>

A collection of items the user has recently played.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

