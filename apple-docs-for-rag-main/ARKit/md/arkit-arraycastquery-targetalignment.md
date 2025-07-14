

- ARKit
- ARRaycastQuery
-  targetAlignment 

Instance Property

# targetAlignment

The target’s alignment with respect to gravity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var targetAlignment: ARRaycastQuery.TargetAlignment { get }
```

## Discussion

The available options are horizontal, vertical, or any.

## See Also

### Specifying the Target

var target: ARRaycastQuery.Target

A plane type that allows the raycast to terminate if it’s encountered.

enum Target

The types of surface you allow a raycast to intersect with.

enum TargetAlignment

A specification that indicates a target’s alignment with respect to gravity

