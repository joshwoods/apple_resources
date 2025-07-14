

- AVFoundation
- AVCaptureScreenInput
-  minFrameDuration 

Instance Property

# minFrameDuration

The screen input’s minimum frame duration.

macOS 10.7+

``` source
var minFrameDuration: CMTime { get set }
```

## Discussion

The `minFrameDuration` is the reciprocal of its maximum frame rate.

You use this property to request a maximum frame rate at which the input produces video frames. The requested rate may not be achievable due to overall bandwidth, so actual frame rates may be lower.

## See Also

### Setting Video Capture Options

var cropRect: CGRect

Indicates the bounding rectangle of the screen area to be captured, in pixels.

var scaleFactor: CGFloat

Indicates the factor by which video buffers captured from the screen are to be scaled.

