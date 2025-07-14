

- ARKit
- ARFaceAnchor
-  rightEyeTransform 

Instance Property

# rightEyeTransform

A transform matrix indicating the position and orientation of the face’s right eye.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var rightEyeTransform: simd_float4x4 { get }
```

## Discussion

The translation aspect of this matrix indicates the position of the center of the eyeball, relative to the position represented by the anchor’s transform. The positive z-axis points from the center of the eyeball in the direction of the pupil.

Rotational aspects of the matrix indicate the orientation of the eyeball—for example, a rotation about the x-axis directs the pupil upward or downward. The eye does not rotate about the z-axis.

## See Also

### Tracking Eye Movement

var leftEyeTransform: simd_float4x4

A transform matrix indicating the position and orientation of the face’s left eye.

var lookAtPoint: simd_float3

A position in face coordinate space estimating the direction of the face’s gaze.

