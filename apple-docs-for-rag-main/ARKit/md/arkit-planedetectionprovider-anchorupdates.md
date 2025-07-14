

- ARKit
- PlaneDetectionProvider
-  anchorUpdates 

Instance Property

# anchorUpdates

A sequence of updates to planes a provider detects.

visionOS 1.0+

``` source
final var anchorUpdates: AnchorUpdateSequence { get }
```

## Discussion

The system adds, updates, or removes plane anchors when this sequence provides updates.

## See Also

### Detecting planes

init(alignments: [PlaneAnchor.Alignment])

Creates a plane detection provider for the types of planes you want to detect.

var allAnchors: [PlaneAnchor]

An array that contains all the plane provider’s anchors.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The types of authorizations necessary for detecting planes.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports plane detection providers.

