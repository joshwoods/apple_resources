

- ARKit
- PlaneDetectionProvider
-  init(alignments:) 

Initializer

# init(alignments:)

Creates a plane detection provider for the types of planes you want to detect.

visionOS 1.0+

``` source
init(alignments: [PlaneAnchor.Alignment] = [.horizontal, .vertical])
```

## Parameters 

`alignments`  

The types of planes you want to detect — horizontal, vertical, or both.

## See Also

### Detecting planes

var allAnchors: [PlaneAnchor]

An array that contains all the plane provider’s anchors.

var anchorUpdates: AnchorUpdateSequence&lt;PlaneAnchor>

A sequence of updates to planes a provider detects.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The types of authorizations necessary for detecting planes.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports plane detection providers.

