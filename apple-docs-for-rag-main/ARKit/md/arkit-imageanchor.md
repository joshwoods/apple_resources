

- ARKit
-  ImageAnchor 

Structure

# ImageAnchor

A 2D image’s position in a person’s surroundings.

visionOS 1.0+

``` source
struct ImageAnchor
```

## Topics

### Getting image information

var originFromAnchorTransform: simd_float4x4

The location and orientation of the image in world space.

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

## Relationships

### Conforms To

- Anchor
- Copyable
- CustomStringConvertible
- Equatable
- Identifiable
- Sendable
- TrackableAnchor

## See Also

### Image tracking

Tracking and altering images

Create images from rectangular shapes found in the user’s environment, and augment their appearance.

Detecting Images in an AR Experience

React to known 2D images in the user’s environment, and use their positions to place AR content.

Tracking preregistered images in 3D space

Place content based on the current position of a known image in a person’s surroundings.

class ImageTrackingProvider

A source of live data about a 2D image’s position in a person’s surroundings.

struct ReferenceImage

A 2D image the system uses as a reference to find the same image in a person’s surroundings.

