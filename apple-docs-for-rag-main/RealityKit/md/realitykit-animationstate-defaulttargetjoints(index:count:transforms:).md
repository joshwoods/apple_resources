

- RealityKit
- AnimationState
-  defaultTargetJoints(index:count:transforms:) 

Instance Method

# defaultTargetJoints(index:count:transforms:)

Retrieves a subset of default target joints, and stores them in the output transform array.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func defaultTargetJoints(
    index: Int,
    count: Int,
    transforms: inout [Transform]
) -> Bool
```

Available when `Value` is `JointTransforms`.

## Discussion

See defaultTarget for more about the default target value.

