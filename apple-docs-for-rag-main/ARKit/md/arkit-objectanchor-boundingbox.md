

- ARKit
- ObjectAnchor
-  boundingBox 

Instance Property

# boundingBox

The bounding box of an anchor.

visionOS 2.0+

``` source
var boundingBox: ObjectAnchor.AxisAlignedBoundingBox { get }
```

## See Also

### Inspecting an object anchor

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

struct ReferenceObject

An object the framework can track.

