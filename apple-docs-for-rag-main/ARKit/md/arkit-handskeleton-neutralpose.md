

- ARKit
- HandSkeleton
-  neutralPose 

Type Property

# neutralPose

A hand pose that you can use as a reference.

visionOS 1.0+

``` source
static var neutralPose: HandSkeleton { get }
```

## Discussion

For example, you might use this property as part of visualizing all of the available joints in a skeleton.

## See Also

### Inspecting hand skeletons

var allJoints: [HandSkeleton.Joint]

All of the joints in a hand skeleton.

var description: String

A textual representation of this Skeleton.

