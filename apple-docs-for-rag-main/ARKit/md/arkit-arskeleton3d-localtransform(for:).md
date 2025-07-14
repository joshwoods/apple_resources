

- ARKit
- ARSkeleton3D
-  localTransform(for:) 

Instance Method

# localTransform(for:)

Returns the local transform for a joint with a given name.

iOS 13.0+iPadOS 13.0+

``` source
@nonobjc
func localTransform(for jointName: ARSkeleton.JointName) -> simd_float4x4?
```

## Discussion

Local space refers to the joints position relative to its parent joint. If an invalid joint name is passed the returned matrix will be filled with `NaN` values.

## See Also

### Getting a Joint’s Pose

var jointLocalTransforms: [simd_float4x4]

The local space transforms for each joint.

var jointModelTransforms: [simd_float4x4]

The model space transforms for each joint.

func modelTransform(for: ARSkeleton.JointName) -> simd_float4x4?

Returns the model transform for a joint with a given name.

