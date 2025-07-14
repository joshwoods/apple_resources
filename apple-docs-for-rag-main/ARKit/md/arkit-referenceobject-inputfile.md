

- ARKit
- ReferenceObject
-  inputFile 

Instance Property

# inputFile

The input file the framework uses for loading a reference object.

visionOS 2.0+

``` source
var inputFile: URL? { get }
```

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

var usdzFile: URL?

The trained USDZ file, if the reference object includes one.

struct ReferenceObject

An object the framework can track.

