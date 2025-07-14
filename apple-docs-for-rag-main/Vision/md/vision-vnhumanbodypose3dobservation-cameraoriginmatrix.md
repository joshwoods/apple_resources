

- Vision
- VNHumanBodyPose3DObservation
-  cameraOriginMatrix 

Instance Property

# cameraOriginMatrix

A transform from the skeleton hip to the camera.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var cameraOriginMatrix: simd_float4x4 { get }
```

## Mentioned in 

Identifying 3D human body poses in images

## See Also

### Getting the Camera Position

func cameraRelativePosition(VNHumanBodyPose3DObservation.JointName) throws -> simd_float4x4

Returns a position relative to the camera for the body joint you specify.

