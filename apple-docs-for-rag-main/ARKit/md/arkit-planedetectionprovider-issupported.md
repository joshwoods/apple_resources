

- ARKit
- PlaneDetectionProvider
-  isSupported 

Type Property

# isSupported

A Boolean value that indicates whether the current runtime environment supports plane detection providers.

visionOS 1.0+

``` source
static var isSupported: Bool { get }
```

## See Also

### Detecting planes

init(alignments: [PlaneAnchor.Alignment])

Creates a plane detection provider for the types of planes you want to detect.

var allAnchors: [PlaneAnchor]

An array that contains all the plane provider’s anchors.

var anchorUpdates: AnchorUpdateSequence&lt;PlaneAnchor>

A sequence of updates to planes a provider detects.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The types of authorizations necessary for detecting planes.

