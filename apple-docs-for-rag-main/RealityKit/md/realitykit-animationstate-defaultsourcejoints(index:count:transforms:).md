

- RealityKit
- AnimationState
-  defaultSourceJoints(index:count:transforms:) 

Instance Method

# defaultSourceJoints(index:count:transforms:)

Retrieves a subset of default source joints, and stores them in the output transform array.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func defaultSourceJoints(
    index: Int,
    count: Int,
    transforms: inout [Transform]
) -> Bool
```

Available when `Value` is `JointTransforms`.

## Discussion

See defaultSource for more about the default source value.

