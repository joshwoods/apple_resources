

- ARKit
- ImageAnchor
-  originFromAnchorTransform 

Instance Property

# originFromAnchorTransform

The location and orientation of the image in world space.

visionOS 1.0+

``` source
var originFromAnchorTransform: simd_float4x4 { get }
```

## See Also

### Getting image information

var referenceImage: ReferenceImage

The reference image that this image anchor tracks.

var estimatedScaleFactor: Float

The estimated scale factor between the tracked image’s physical size and the reference image’s size.

var isTracked: Bool

A Boolean value that indicates whether ARKit is currently tracking this image.

var description: String

A textual representation of this anchor.

var id: UUID

The unique identifier of this anchor.

