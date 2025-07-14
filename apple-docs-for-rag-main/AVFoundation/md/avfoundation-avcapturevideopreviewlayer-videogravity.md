

- AVFoundation
- AVCaptureVideoPreviewLayer
-  videoGravity 

Instance Property

# videoGravity

A value that indicates how the layer displays video content within its bounds.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var videoGravity: AVLayerVideoGravity { get set }
```

## Discussion

Options are resizeAspect, resizeAspectFill, and resize. The default is resizeAspect.

This property is animatable.

## See Also

### Layer Configuration

var isPreviewing: Bool

A Boolean value that indicates whether the layer is rendering video frames from its source.

