

- ARKit
- ObjectTrackingProvider
-  allAnchors 

Instance Property

# allAnchors

An array of all the object anchors the object-tracking provider is tracking.

visionOS 2.0+

``` source
final var allAnchors: [ObjectAnchor] { get }
```

## See Also

### Inspecting an object-tracking provider

var state: DataProviderState

The state of an object-tracking provider.

var anchorUpdates: AnchorUpdateSequence&lt;ObjectAnchor>

An asynchronous sequence of anchors the framework updates.

struct Error

Values that represent an object-tracking error.

var description: String

A textual representation of this object tracking provider.

