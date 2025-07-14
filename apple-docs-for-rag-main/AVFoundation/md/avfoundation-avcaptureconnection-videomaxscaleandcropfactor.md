

- AVFoundation
- AVCaptureConnection
-  videoMaxScaleAndCropFactor 

Instance Property

# videoMaxScaleAndCropFactor

The connection’s maximum video scale and crop factor.

iOS 5.0+iPadOS 5.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var videoMaxScaleAndCropFactor: CGFloat { get }
```

## Discussion

The value defines the largest value you can set the videoScaleAndCropFactor property to, which only applies to a video connection.

## See Also

### Scaling a video

var videoScaleAndCropFactor: CGFloat

The current scale and crop factor the video output uses.

