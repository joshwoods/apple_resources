

- AVFoundation
- AVCaptureConnection
-  videoFieldMode 

Instance Property

# videoFieldMode

A setting that tells the connection how to interlace video flowing through it.

macOS 10.7+

``` source
var videoFieldMode: AVVideoFieldMode { get set }
```

## Discussion

The property only applies to a video connection and when isVideoFieldModeSupported is true.

## See Also

### Interlacing video

var isVideoFieldModeSupported: Bool

A Boolean value that indicates whether the connection supports setting a video field mode.

enum AVVideoFieldMode

Constants that indicate which interlacing modes the connection applies to video flowing through it.

