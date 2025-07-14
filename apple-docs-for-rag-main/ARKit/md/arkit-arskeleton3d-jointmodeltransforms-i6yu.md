

- ARKit
- ARSkeleton3D
-  jointModelTransforms 

Instance Property

# jointModelTransforms

The model space transforms for each joint.

iOS 13.0+iPadOS 13.0+

``` source
@nonobjc
var jointModelTransforms: [simd_float4x4] { get }
```

## Discussion

Model space refers to a joint’s position relative to the hip joint. Note, the hip joint is located at the body anchor’s origin.

## See Also

### Getting a Joint’s Pose

var jointLocalTransforms: [simd_float4x4]

The local space transforms for each joint.

func localTransform(for: ARSkeleton.JointName) -> simd_float4x4?

Returns the local transform for a joint with a given name.

func modelTransform(for: ARSkeleton.JointName) -> simd_float4x4?

Returns the model transform for a joint with a given name.

