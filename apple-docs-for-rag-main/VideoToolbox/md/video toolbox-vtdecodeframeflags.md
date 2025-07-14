

- Video Toolbox
-  VTDecodeFrameFlags 

Structure

# VTDecodeFrameFlags

Flags to pass to a decompression session and the video decoder.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
struct VTDecodeFrameFlags
```

## Topics

### Flags

init(rawValue: UInt32)

Creates a flags structure with a raw value.

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

struct VTDecodeInfoFlags

Flags that provide information about the status of a decode operation.

typealias VTDecompressionOutputCallback

The prototype for the callback invoked when frame decompression is complete.

struct VTDecompressionOutputCallbackRecord

typealias VTDecompressionOutputHandler

The prototype for the block invoked when frame decompression is complete.

