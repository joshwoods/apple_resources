

- ARKit
- ARSkeletonDefinition
-  jointCount 

Instance Property

# jointCount

The skeleton’s total number of joints.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var jointCount: Int { get }
```

## See Also

### Getting Joint Information

var jointNames: [String]

A collection of unique joint names.

func index(for: ARSkeleton.JointName) -> Int

Returns the index for a given joint identifier.

var parentIndices: [Int]

The parent index for each joint.

