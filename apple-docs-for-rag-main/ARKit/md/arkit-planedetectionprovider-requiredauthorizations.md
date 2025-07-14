

- ARKit
- PlaneDetectionProvider
-  requiredAuthorizations 

Type Property

# requiredAuthorizations

The types of authorizations necessary for detecting planes.

visionOS 1.0+

``` source
static var requiredAuthorizations: [ARKitSession.AuthorizationType] { get }
```

## Discussion

You can use this property to pass plane detection requirements to the requestAuthorization(for:) method.

## See Also

### Detecting planes

init(alignments: [PlaneAnchor.Alignment])

Creates a plane detection provider for the types of planes you want to detect.

var allAnchors: [PlaneAnchor]

An array that contains all the plane provider’s anchors.

var anchorUpdates: AnchorUpdateSequence&lt;PlaneAnchor>

A sequence of updates to planes a provider detects.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports plane detection providers.

