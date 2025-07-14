

- ARKit
- PlaneDetectionProvider
-  allAnchors 

Instance Property

# allAnchors

An array that contains all the plane provider’s anchors.

visionOS 2.0+

``` source
final var allAnchors: [PlaneAnchor] { get }
```

## See Also

### Detecting planes

init(alignments: [PlaneAnchor.Alignment])

Creates a plane detection provider for the types of planes you want to detect.

var anchorUpdates: AnchorUpdateSequence&lt;PlaneAnchor>

A sequence of updates to planes a provider detects.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The types of authorizations necessary for detecting planes.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports plane detection providers.

