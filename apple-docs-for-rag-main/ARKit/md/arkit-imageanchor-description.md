

- ARKit
- ImageAnchor
-  description 

Instance Property

# description

A textual representation of this anchor.

visionOS 1.0+

``` source
var description: String { get }
```

## See Also

### Getting image information

var originFromAnchorTransform: simd_float4x4

The location and orientation of the image in world space.

var referenceImage: ReferenceImage

The reference image that this image anchor tracks.

var estimatedScaleFactor: Float

The estimated scale factor between the tracked image’s physical size and the reference image’s size.

var isTracked: Bool

A Boolean value that indicates whether ARKit is currently tracking this image.

var id: UUID

The unique identifier of this anchor.

