

- AVFoundation
- AVCameraCalibrationData
-  lensDistortionCenter 

Instance Property

# lensDistortionCenter

The offset of the distortion center of the camera lens from the top-left corner of the image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var lensDistortionCenter: CGPoint { get }
```

## Discussion

Due to geometric distortions in the image, the center of the distortion may not be equal to the optical center (principal point) of the lens. When making an image rectilinear, use the distortion center rather than the optical center of the image.

## See Also

### Correcting for Lens Distortion

var lensDistortionLookupTable: Data?

A map of floating-point values describing radial distortions imparted by the camera lens, for use in rectifying camera images.

var inverseLensDistortionLookupTable: Data?

A map of floating-point values describing radial distortions for use in reapplying camera geometry to a rectified image.

