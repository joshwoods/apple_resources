

- ARKit
-  PlaneAnchor 

Structure

# PlaneAnchor

An anchor that represents horizontal and vertical planes.

visionOS 1.0+

``` source
struct PlaneAnchor
```

## Topics

### Inspecting a plane anchor

var originFromAnchorTransform: simd_float4x4

The location and orientation of a plane in world space.

var alignment: PlaneAnchor.Alignment

The general orientation of the detected plane with respect to gravity.

enum Alignment

Values describing possible general orientations of a detected plane with respect to gravity.

var classification: PlaneAnchor.Classification

Get the classification of this plane.

enum Classification

The kinds of object classification a plane anchor can have.

var description: String

A textual representation of this anchor.

### Getting the shape of a plane anchor

var geometry: PlaneAnchor.Geometry

Get the geometry of the plane in the anchor’s coordinate system.

struct Geometry

The geometry of a plane anchor.

### Identifying a plane anchor

var id: UUID

The unique identifier of this anchor.

## Relationships

### Conforms To

- Anchor
- Copyable
- CustomStringConvertible
- Equatable
- Identifiable
- Sendable

## See Also

### Plane detection

Placing content on detected planes

Detect horizontal surfaces like tables and floors, as well as vertical planes like walls and doors.

class PlaneDetectionProvider

A source of live data about planes in a person’s surroundings.

