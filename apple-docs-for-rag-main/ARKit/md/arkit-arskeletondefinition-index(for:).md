

- ARKit
- ARSkeletonDefinition
-  index(for:) 

Instance Method

# index(for:)

Returns the index for a given joint identifier.

iOS 13.0+iPadOS 13.0+

``` source
@nonobjc
func index(for jointName: ARSkeleton.JointName) -> Int
```

## Discussion

This function returns `NSNotFound` if an invalid joint name is passed in.

## See Also

### Getting Joint Information

var jointNames: [String]

A collection of unique joint names.

var jointCount: Int

The skeleton’s total number of joints.

var parentIndices: [Int]

The parent index for each joint.

