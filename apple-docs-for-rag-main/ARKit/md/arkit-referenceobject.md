

- ARKit
-  ReferenceObject 

Structure

# ReferenceObject

An object the framework can track.

visionOS 2.0+

``` source
struct ReferenceObject
```

## Topics

### Creating reference objects

init(from: URL) async throws

Creates a reference object from a URL you provide.

init(named: String, from: Bundle?) async throws

Creates a reference object from a bundle.

### Inspecting a reference object

var id: UUID

The unique identifier of this anchor.

typealias ID

A type representing the stable identity of the entity associated with an instance.

var inputFile: URL?

The input file the framework uses for loading a reference object.

var usdzFile: URL?

The trained USDZ file, if the reference object includes one.

var name: String

The name of a reference object.

var description: String

A textual representation of this reference object.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Identifiable
- Sendable

## See Also

### Inspecting an object anchor

var boundingBox: ObjectAnchor.AxisAlignedBoundingBox

The bounding box of an anchor.

struct AxisAlignedBoundingBox

Values that describe an axis-aligned bounding box.

var description: String

A textual representation of this anchor.

var isTracked: Bool

A Boolean value that indicates whether the framework is currently tracking an object anchor.

var originFromAnchorTransform: simd_float4x4

The transform from the object anchor to the origin coordinate system.

var referenceObject: ReferenceObject

The reference object that an anchor corresponds to.

var inputFile: URL?

The input file the framework uses for loading a reference object.

var usdzFile: URL?

The trained USDZ file, if the reference object includes one.

