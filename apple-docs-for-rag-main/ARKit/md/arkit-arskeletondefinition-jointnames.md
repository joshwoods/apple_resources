

- ARKit
- ARSkeletonDefinition
-  jointNames 

Instance Property

# jointNames

A collection of unique joint names.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var jointNames: [String] { get }
```

## Discussion

Refer to this array to convert a joint index to a joint identifier.

## See Also

### Getting Joint Information

var jointCount: Int

The skeleton’s total number of joints.

func index(for: ARSkeleton.JointName) -> Int

Returns the index for a given joint identifier.

var parentIndices: [Int]

The parent index for each joint.

