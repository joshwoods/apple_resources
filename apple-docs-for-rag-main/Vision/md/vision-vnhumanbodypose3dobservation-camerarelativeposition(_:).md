

- Vision
- VNHumanBodyPose3DObservation
-  cameraRelativePosition(\_:) 

Instance Method

# cameraRelativePosition(\_:)

Returns a position relative to the camera for the body joint you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
@nonobjc
func cameraRelativePosition(_ jointName: VNHumanBodyPose3DObservation.JointName) throws -> simd_float4x4
```

## Parameters 

`jointName`  

The name of the human body joint.

## Return Value

The joint position, in meters.

## Mentioned in 

Identifying 3D human body poses in images

## See Also

### Getting the Camera Position

var cameraOriginMatrix: simd_float4x4

A transform from the skeleton hip to the camera.

