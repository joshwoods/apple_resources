

- RealityKit
- AnimationState
-  storeAnimatedJoints(transforms:jointIndex:) 

Instance Method

# storeAnimatedJoints(transforms:jointIndex:)

Stores a subset of animated joints.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@discardableResult
func storeAnimatedJoints(
    transforms: [Transform],
    jointIndex: Int
) -> Bool
```

Available when `Value` is `JointTransforms`.

## Discussion

See storeAnimatedValue(_:) for more about returning an animation result to the animation system.

