

- RealityKit
- AudioFileResource
-  AudioFileResource.LoadingStrategy 

Enumeration

# AudioFileResource.LoadingStrategy

A container for different strategies on how to handle resources’ data before and during playback.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
enum LoadingStrategy
```

## Topics

### Specifying a loading strategy

case preload

Load and decode all the data into memory before playback.

case stream

Stream data from disk, decoding in real time.

### Comparing loading strategies

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting types

struct Configuration

A container for various settings for loading an audio file resource.

