

- ARKit
- ARRaycastQuery
-  target 

Instance Property

# target

A plane type that allows the raycast to terminate if it’s encountered.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var target: ARRaycastQuery.Target { get }
```

## Discussion

The available target types are plane, infinite plane, and estimated plane.

## See Also

### Specifying the Target

enum Target

The types of surface you allow a raycast to intersect with.

var targetAlignment: ARRaycastQuery.TargetAlignment

The target’s alignment with respect to gravity.

enum TargetAlignment

A specification that indicates a target’s alignment with respect to gravity

