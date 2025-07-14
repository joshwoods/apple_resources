

- Media Player
-  MPNowPlayingInfoMediaType 

Enumeration

# MPNowPlayingInfoMediaType

The type of media currently playing.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 10.0+visionOS 1.0+watchOS 5.0+

``` source
enum MPNowPlayingInfoMediaType
```

## Topics

### Enumeration Cases

case none

There is no now playing media item.

case audio

The now playing media item is an audio item.

case none

There is no now playing media item.

case video

The now playing media item is a video item.

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

### Working with the default Now Playing info center

class func `default`() -> MPNowPlayingInfoCenter

Returns the singleton Now Playing info center.

var nowPlayingInfo: [String : Any]?

The current Now Playing information for the default Now Playing info center.

