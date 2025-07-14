

- ARKit
- PlaneAnchor
-  PlaneAnchor.Alignment 

Enumeration

# PlaneAnchor.Alignment

Values describing possible general orientations of a detected plane with respect to gravity.

visionOS 1.0+

``` source
enum Alignment
```

## Topics

### Alignment Values

case horizontal

The plane is in a horizontal oriention.

case vertical

The plane is in a vertical orientation.

### Enumeration Cases

case slanted

The plane is in a slanted orientation.

### Instance Properties

var description: String

A textual representation of PlaneAnchor.Alignment

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting a plane anchor

var originFromAnchorTransform: simd_float4x4

The location and orientation of a plane in world space.

var alignment: PlaneAnchor.Alignment

The general orientation of the detected plane with respect to gravity.

var classification: PlaneAnchor.Classification

Get the classification of this plane.

enum Classification

The kinds of object classification a plane anchor can have.

var description: String

A textual representation of this anchor.

