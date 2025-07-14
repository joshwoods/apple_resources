

- Video Toolbox
-  VTDecompressionSession 

Class

# VTDecompressionSession

A reference to a decompression session.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
class VTDecompressionSession
```

## Overview

A decompression session supports the decompression of a sequence of video frames. The session is a reference-counted Core Foundation (CF) object.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Data Types

struct VTDecodeFrameFlags

Flags to pass to a decompression session and the video decoder.

struct VTDecodeInfoFlags

Flags that provide information about the status of a decode operation.

typealias VTDecompressionOutputCallback

The prototype for the callback invoked when frame decompression is complete.

struct VTDecompressionOutputCallbackRecord

typealias VTDecompressionOutputHandler

The prototype for the block invoked when frame decompression is complete.

