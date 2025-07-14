

- ARKit
-  ReferenceImage 

Structure

# ReferenceImage

A 2D image the system uses as a reference to find the same image in a person’s surroundings.

visionOS 1.0+

``` source
struct ReferenceImage
```

## Topics

### Creating a reference image

init(cgimage: CGImage, physicalSize: CGSize, orientation: CGImagePropertyOrientation)

Creates a reference image from a Core Graphics image.

init(pixelBuffer: CVPixelBuffer, physicalSize: CGSize, orientation: CGImagePropertyOrientation)

Creates a reference image from a pixel buffer.

static func loadReferenceImages(inGroupNamed: String, bundle: Bundle?) -> [ReferenceImage]

Creates multiple reference images based on their group name in an asset catalog.

### Inspecting a reference image

var physicalSize: CGSize

The size, in meters, of a reference image in the real world.

var name: String?

The name of a reference image.

var resourceGroupName: String?

A string value the represents the name of the resource group the framework loads an image from.

var description: String

A textual representation of this reference image.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Sendable

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

struct ImageAnchor

A 2D image’s position in a person’s surroundings.

