

- ARKit
-  ImageTrackingProvider 

Class

# ImageTrackingProvider

A source of live data about a 2D image’s position in a person’s surroundings.

visionOS 1.0+

``` source
final class ImageTrackingProvider
```

## Topics

### Creating an image-tracking provider

init(referenceImages: [ReferenceImage])

Creates an image-tracking provider that tracks the reference images you supply.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports image-tracking providers.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The types of authorizations necessary for tracking images.

### Tracking images

var anchorUpdates: AnchorUpdateSequence&lt;ImageAnchor>

A sequence of updates that provide information about images a provider tracks.

### Inspecting an image-tracking provider

var state: DataProviderState

The current status of data coming from a provider.

var description: String

A textual representation of this image tracking provider.

var allAnchors: [ImageAnchor]

An array of all the image anchors the provider is tracking.

## Relationships

### Conforms To

- CustomStringConvertible
- DataProvider
- Sendable

## See Also

### Image tracking

Tracking and altering images

Create images from rectangular shapes found in the user’s environment, and augment their appearance.

Detecting Images in an AR Experience

React to known 2D images in the user’s environment, and use their positions to place AR content.

Tracking preregistered images in 3D space

Place content based on the current position of a known image in a person’s surroundings.

struct ImageAnchor

A 2D image’s position in a person’s surroundings.

struct ReferenceImage

A 2D image the system uses as a reference to find the same image in a person’s surroundings.

