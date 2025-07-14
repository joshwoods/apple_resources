

- Video Toolbox
-  VTDecompressionOutputCallbackRecord 

Structure

# VTDecompressionOutputCallbackRecord

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
struct VTDecompressionOutputCallbackRecord
```

## Topics

### Initializers

init()

init(decompressionOutputCallback: VTDecompressionOutputCallback?, decompressionOutputRefCon: UnsafeMutableRawPointer?)

### Instance Properties

var decompressionOutputCallback: VTDecompressionOutputCallback?

var decompressionOutputRefCon: UnsafeMutableRawPointer?

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

class VTDecompressionSession

A reference to a decompression session.

struct VTDecodeFrameFlags

Flags to pass to a decompression session and the video decoder.

struct VTDecodeInfoFlags

Flags that provide information about the status of a decode operation.

typealias VTDecompressionOutputCallback

The prototype for the callback invoked when frame decompression is complete.

typealias VTDecompressionOutputHandler

The prototype for the block invoked when frame decompression is complete.

