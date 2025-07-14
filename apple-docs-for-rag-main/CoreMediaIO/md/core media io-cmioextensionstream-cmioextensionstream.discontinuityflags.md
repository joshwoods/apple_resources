

- Core Media I/O
- CMIOExtensionStream
-  CMIOExtensionStream.DiscontinuityFlags 

Structure

# CMIOExtensionStream.DiscontinuityFlags

Constants that specify the types of discontinuities that can occur in a media stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
struct DiscontinuityFlags
```

## Topics

### Discontinuity Flags

static var unknown: CMIOExtensionStream.DiscontinuityFlags

A flag that indicates a stream discontinuity due to an unknown reason.

static var time: CMIOExtensionStream.DiscontinuityFlags

A flag that indicates a time discontinuity in the stream.

static var sampleDropped: CMIOExtensionStream.DiscontinuityFlags

A flag that indicates a discontinuity in the stream due to a dropped frame.

### Initializers

init(rawValue: UInt32)

Creates a flag with an integer value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Processing Data

func consumeSampleBuffer(from: CMIOExtensionClient, completionHandler: (CMSampleBuffer?, UInt64, CMIOExtensionStream.DiscontinuityFlags, Bool, (any Error)?) -> Void)

Consumes a sample buffer from a client.

func send(CMSampleBuffer, discontinuity: CMIOExtensionStream.DiscontinuityFlags, hostTimeInNanoseconds: UInt64)

Sends a media sample to stream client.

