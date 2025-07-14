

- AVFoundation
- AVCaptureConnection
-  isVideoFieldModeSupported 

Instance Property

# isVideoFieldModeSupported

A Boolean value that indicates whether the connection supports setting a video field mode.

macOS 10.7+

``` source
var isVideoFieldModeSupported: Bool { get }
```

## Discussion

The property only applies to a video connection’s videoFieldMode property.

## See Also

### Interlacing video

var videoFieldMode: AVVideoFieldMode

A setting that tells the connection how to interlace video flowing through it.

enum AVVideoFieldMode

Constants that indicate which interlacing modes the connection applies to video flowing through it.

