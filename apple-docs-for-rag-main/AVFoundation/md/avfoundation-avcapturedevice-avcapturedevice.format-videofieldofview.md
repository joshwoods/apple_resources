

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  videoFieldOfView 

Instance Property

# videoFieldOfView

Indicates the format’s horizontal field of view in degrees.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var videoFieldOfView: Float { get }
```

## Discussion

Returns zero if the format’s field of view is unknown.

## See Also

### Determining Field of View

var geometricDistortionCorrectedVideoFieldOfView: Float

A horizontal field of view for the format after correction for geometric distortion.

