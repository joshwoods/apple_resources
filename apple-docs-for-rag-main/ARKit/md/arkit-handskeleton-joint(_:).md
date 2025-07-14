

- ARKit
- HandSkeleton
-  joint(\_:) 

Instance Method

# joint(\_:)

Retrieves a hand joint based on the joint name you specify.

visionOS 1.0+

``` source
func joint(_ named: HandSkeleton.JointName) -> HandSkeleton.Joint
```

## Parameters 

`named`  

The name of the hand joint to retrieve.

## Return Value

A hand joint referred to by the `named` parameter.

## See Also

### Retrieving specific hand joints

struct Joint

The name and position of an individual hand joint.

enum JointName

The names of different hand joints.

