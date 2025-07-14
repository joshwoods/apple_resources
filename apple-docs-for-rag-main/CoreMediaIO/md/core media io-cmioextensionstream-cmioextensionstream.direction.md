

- Core Media I/O
- CMIOExtensionStream
-  CMIOExtensionStream.Direction 

Enumeration

# CMIOExtensionStream.Direction

Constants that define the data-flow direction of the stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
enum Direction
```

## Overview

A stream can be a source or sink. A source stream produces samples, and a sink stream consumes samples.

## Topics

### Directions

case source

A stream that provides sample buffers for capture.

case sink

A stream that consumes sample buffers for playback.

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

### Inspecting a Stream

var source: (any CMIOExtensionStreamSource)?

The source object for the stream.

var direction: CMIOExtensionStream.Direction

The data-flow direction of the stream.

var clockType: CMIOExtensionStream.ClockType

A clock type for the stream.

enum ClockType

Constants that indicate the clock type of a stream.

var customClockConfiguration: CMIOExtensionStreamCustomClockConfiguration?

An optional custom clock configuration for a stream.

class CMIOExtensionStreamCustomClockConfiguration

An object that describes the parameters to create a custom clock on the host side.

