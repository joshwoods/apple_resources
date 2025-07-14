

- ARKit
- ARSkeleton
-  isJointTracked(\_:) 

Instance Method

# isJointTracked(\_:)

Tells you whether ARKit tracks a joint at a particular index.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func isJointTracked(_ jointIndex: Int) -> Bool
```

## Discussion

Use this function to determine which joints ARKit tracks using a particular index.

## See Also

### Getting Joint Information

var definition: ARSkeletonDefinition

The particular configuration of joints that define a body’s current state.

struct JointName

A name identifier for a joint.

