

- ARKit
- ObjectAnchor
-  ObjectAnchor.AxisAlignedBoundingBox 

Structure

# ObjectAnchor.AxisAlignedBoundingBox

Values that describe an axis-aligned bounding box.

visionOS 2.0+

``` source
struct AxisAlignedBoundingBox
```

## Topics

### Inspecting the bounding box

var center: SIMD3&lt;Float>

The center of the bounding box.

var extent: SIMD3&lt;Float>

The extent of the bounding box.

var max: SIMD3&lt;Float>

The maximum coordinates for the bounding box.

var min: SIMD3&lt;Float>

Minimum coordinates for the bounding box.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Inspecting an object anchor

var boundingBox: ObjectAnchor.AxisAlignedBoundingBox

The bounding box of an anchor.

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

struct ReferenceObject

An object the framework can track.

