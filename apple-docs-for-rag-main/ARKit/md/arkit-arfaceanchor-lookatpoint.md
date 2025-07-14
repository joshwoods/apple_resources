

- ARKit
- ARFaceAnchor
-  lookAtPoint 

Instance Property

# lookAtPoint

A position in face coordinate space estimating the direction of the face’s gaze.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var lookAtPoint: simd_float3 { get }
```

## Discussion

This vector abstracts from the leftEyeTransform and rightEyeTransform matrices to estimate what point, relative to the face, the user’s eyes are focused upon. For example:

- If the user is looking to the left, the vector has a positive x-axis component.

- If the user is focused on a nearby object, the vector’s length is shorter.

- If the user is focused on a faraway object, the vector’s length is longer.

## See Also

### Tracking Eye Movement

var leftEyeTransform: simd_float4x4

A transform matrix indicating the position and orientation of the face’s left eye.

var rightEyeTransform: simd_float4x4

A transform matrix indicating the position and orientation of the face’s right eye.

