

- ARKit
- PlaneAnchor
-  PlaneAnchor.Classification 

Enumeration

# PlaneAnchor.Classification

The kinds of object classification a plane anchor can have.

visionOS 1.0+

``` source
enum Classification
```

## Topics

### Getting known classifications

case ceiling

A ceiling.

case door

A door.

case floor

A floor.

case seat

A seat.

case table

A table.

case wall

A wall.

case window

A window.

### Getting unknown classifications

case notAvailable

A plane classification is currently unavailable.

case undetermined

A plane classification hasn’t been determined yet.

case unknown

A plane classification isn’t one of the known classes.

### Instance Properties

var description: String

A textual representation of PlaneAnchor.Classification

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

enum Alignment

Values describing possible general orientations of a detected plane with respect to gravity.

var classification: PlaneAnchor.Classification

Get the classification of this plane.

var description: String

A textual representation of this anchor.

