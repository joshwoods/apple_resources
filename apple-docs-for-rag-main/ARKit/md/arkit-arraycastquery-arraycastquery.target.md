

- ARKit
- ARRaycastQuery
-  ARRaycastQuery.Target 

Enumeration

# ARRaycastQuery.Target

The types of surface you allow a raycast to intersect with.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
enum Target
```

## Discussion

The available target types are plane, infinite plane, and estimated plane.

## Topics

### Targets

case estimatedPlane

A raycast target that specifies nonplanar surfaces, or planes about which ARKit can only estimate.

case existingPlaneGeometry

A raycast target that requires a plane to have a definitive size and shape.

case existingPlaneInfinite

A raycast target that specifies a detected plane, regardless of its size and shape.

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

var targetAlignment: ARRaycastQuery.TargetAlignment

The target’s alignment with respect to gravity.

enum TargetAlignment

A specification that indicates a target’s alignment with respect to gravity

