

- RealityKit
- SkeletalPose
-  jointTransforms 

Instance Property

# jointTransforms

The transformations of the joints in the pose.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var jointTransforms: JointTransforms
```

## Discussion

Each joint transformation has a corresponding name in jointNames at the same index.

A new value with element count not matching the element count of jointNames is accepted but invokes special handling when the SkeletalPosesComponent is set on an entity.

