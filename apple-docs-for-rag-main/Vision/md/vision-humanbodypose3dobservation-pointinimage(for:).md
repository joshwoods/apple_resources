

- Vision
- HumanBodyPose3DObservation
-  pointInImage(for:) 

Instance Method

# pointInImage(for:)

Returns a 2D point for the joint name you specify, relative to the input image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func pointInImage(for jointName: HumanBodyPose3DObservation.JointName) -> NormalizedPoint
```

## Parameters 

`jointName`  

The name of the human body joint.

## Return Value

A projection of the 3D position onto the original 2D image in normalized, lower left origin coordinates.

