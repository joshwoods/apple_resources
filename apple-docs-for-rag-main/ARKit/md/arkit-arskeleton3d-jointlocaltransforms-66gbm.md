

- ARKit
- ARSkeleton3D
-  jointLocalTransforms 

Instance Property

# jointLocalTransforms

The local space transforms for each joint.

iOS 13.0+iPadOS 13.0+

``` source
@nonobjc
var jointLocalTransforms: [simd_float4x4] { get }
```

## Discussion

Local space refers to a joint’s position relative to its parent joint.

## See Also

### Getting a Joint’s Pose

var jointModelTransforms: [simd_float4x4]

The model space transforms for each joint.

func localTransform(for: ARSkeleton.JointName) -> simd_float4x4?

Returns the local transform for a joint with a given name.

func modelTransform(for: ARSkeleton.JointName) -> simd_float4x4?

Returns the model transform for a joint with a given name.

