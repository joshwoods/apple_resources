

- RealityKit
- SkeletalPose
-  jointNames 

Instance Property

# jointNames

The names of the joints in the pose in specific order.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var jointNames: [String] { get set }
```

## Discussion

Each joint name has a corresponding transformation value in jointTransforms at the same index.

Updates of the value results in resizing or reordering of the pose’s jointTransforms to match. New joint names add identity transformations at the matching indices.

