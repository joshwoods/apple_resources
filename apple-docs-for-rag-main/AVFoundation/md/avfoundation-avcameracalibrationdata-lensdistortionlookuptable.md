

- AVFoundation
- AVCameraCalibrationData
-  lensDistortionLookupTable 

Instance Property

# lensDistortionLookupTable

A map of floating-point values describing radial distortions imparted by the camera lens, for use in rectifying camera images.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var lensDistortionLookupTable: Data? { get }
```

## Discussion

Images captured by a camera are geometrically warped by small imperfections in the lens. To project from the 2D image plane back into the 3D world, the images must be distortion corrected, or made rectilinear. Lens distortion is modeled using a one-dimensional lookup table of 32-bit float values evenly distributed along a radius from the center of the distortion to a corner, with each value representing a magnification of the radius. This model assumes symmetrical lens distortion.

When dealing with AVDepthData objects, the disparity/depth map representations are geometrically distorted to align with images produced by the camera.

## See Also

### Correcting for Lens Distortion

var inverseLensDistortionLookupTable: Data?

A map of floating-point values describing radial distortions for use in reapplying camera geometry to a rectified image.

var lensDistortionCenter: CGPoint

The offset of the distortion center of the camera lens from the top-left corner of the image.

