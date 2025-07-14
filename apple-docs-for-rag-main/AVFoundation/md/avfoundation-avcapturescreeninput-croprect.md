

- AVFoundation
- AVCaptureScreenInput
-  cropRect 

Instance Property

# cropRect

Indicates the bounding rectangle of the screen area to be captured, in pixels.

macOS 10.7+

``` source
var cropRect: CGRect { get set }
```

## Discussion

By default, `AVCaptureScreenInput` captures the entire area of the displayID with which it is associated.

Set the value of this property to limit the capture rectangle to a subsection of the screen.

The rectangle should define a smaller section of the screen in the screen’s coordinate system. The origin (0,0) is the bottom-left corner of the screen.

## See Also

### Setting Video Capture Options

var minFrameDuration: CMTime

The screen input’s minimum frame duration.

var scaleFactor: CGFloat

Indicates the factor by which video buffers captured from the screen are to be scaled.

