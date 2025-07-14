

- ARKit
- ARSkeleton3D
-  modelTransform(for:) 

Instance Method

# modelTransform(for:)

Returns the model transform for a joint with a given name.

iOS 13.0+iPadOS 13.0+

``` source
@nonobjc
func modelTransform(for jointName: ARSkeleton.JointName) -> simd_float4x4?
```

## Discussion

Model space refers to the joint’s position relative to its hip joint. If an invalid joint name is passed in, the returned matrix will be filled with `NaN` values.

## See Also

### Getting a Joint’s Pose

var jointLocalTransforms: [simd_float4x4]

The local space transforms for each joint.

var jointModelTransforms: [simd_float4x4]

The model space transforms for each joint.

func localTransform(for: ARSkeleton.JointName) -> simd_float4x4?

Returns the local transform for a joint with a given name.

