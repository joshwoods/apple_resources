

- MediaExtension
-  MEDecodeFrameStatus 

Structure

# MEDecodeFrameStatus

A type that represents a non-error status related to a frame decode operation.

macOS 14.0+

``` source
struct MEDecodeFrameStatus
```

## Topics

### Creating a status

init(rawValue: UInt)

Creates a new frame decode operation status with the raw value that you specify.

### Inspecting a status

static var frameDropped: MEDecodeFrameStatus

A frame decode operation status that indicates the system dropped the output of the frame for a reason other than an error.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

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

### Decoding frames

func canAccept(CMFormatDescription) -> Bool

Asks the extension whether the decoder can decode frames with the format description that you specify.

func decodeFrame(from: CMSampleBuffer, options: MEDecodeFrameOptions, completionHandler: (CVImageBuffer?, MEDecodeFrameStatus, (any Error)?) -> Void)

Requests the extension to decode a video frame.

**Required**

