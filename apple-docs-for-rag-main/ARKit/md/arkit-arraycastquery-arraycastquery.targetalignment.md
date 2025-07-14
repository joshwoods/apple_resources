

- ARKit
- ARRaycastQuery
-  ARRaycastQuery.TargetAlignment 

Enumeration

# ARRaycastQuery.TargetAlignment

A specification that indicates a target’s alignment with respect to gravity

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
enum TargetAlignment
```

## Discussion

A raycast ignores potential targets with an alignment different than the one you specify in the raycast query.

## Topics

### Enumeration Cases

case any

The case that indicates a target may be aligned in any way with respect to gravity.

case horizontal

The case that indicates a target is aligned horizontally with respect to gravity.

case vertical

The case that indicates a target is aligned vertically with respect to gravity.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the Target

var target: ARRaycastQuery.Target

A plane type that allows the raycast to terminate if it’s encountered.

enum Target

The types of surface you allow a raycast to intersect with.

var targetAlignment: ARRaycastQuery.TargetAlignment

The target’s alignment with respect to gravity.

