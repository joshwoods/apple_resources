

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  geometricDistortionCorrectedVideoFieldOfView 

Instance Property

# geometricDistortionCorrectedVideoFieldOfView

A horizontal field of view for the format after correction for geometric distortion.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var geometricDistortionCorrectedVideoFieldOfView: Float { get }
```

## Discussion

If the capture device doesn’t support geometric distortion correction (GDC), the value of this property is equal to the value of videoFieldOfView.

## See Also

### Determining Field of View

var videoFieldOfView: Float

Indicates the format’s horizontal field of view in degrees.

