

- ARKit
- ImageAnchor
-  isTracked 

Instance Property

# isTracked

A Boolean value that indicates whether ARKit is currently tracking this image.

visionOS 1.0+

``` source
var isTracked: Bool { get }
```

## See Also

### Getting image information

var originFromAnchorTransform: simd_float4x4

The location and orientation of the image in world space.

var referenceImage: ReferenceImage

The reference image that this image anchor tracks.

var estimatedScaleFactor: Float

The estimated scale factor between the tracked image’s physical size and the reference image’s size.

var description: String

A textual representation of this anchor.

var id: UUID

The unique identifier of this anchor.

