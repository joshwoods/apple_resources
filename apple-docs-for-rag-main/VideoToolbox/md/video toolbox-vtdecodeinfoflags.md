

- Video Toolbox
-  VTDecodeInfoFlags 

Structure

# VTDecodeInfoFlags

Flags that provide information about the status of a decode operation.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
struct VTDecodeInfoFlags
```

## Topics

### Flag values

static var asynchronous: VTDecodeInfoFlags

A flag that indicates the decode operation ran asynchronously.

static var frameDropped: VTDecodeInfoFlags

A flag that indicates the decode operation dropped a frame.

static var skippedLeadingFrameDropped: VTDecodeInfoFlags

A flag that indicates whether the decode process skips leading frames after dropping a synchronization frame.

static var imageBufferModifiable: VTDecodeInfoFlags

A flag that indicates the image buffer is safe to modify.

### Initializers

init(rawValue: UInt32)

Creates a flag from a raw unsigned-integer value.

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

### Data Types

class VTDecompressionSession

A reference to a decompression session.

struct VTDecodeFrameFlags

Flags to pass to a decompression session and the video decoder.

typealias VTDecompressionOutputCallback

The prototype for the callback invoked when frame decompression is complete.

struct VTDecompressionOutputCallbackRecord

typealias VTDecompressionOutputHandler

The prototype for the block invoked when frame decompression is complete.

