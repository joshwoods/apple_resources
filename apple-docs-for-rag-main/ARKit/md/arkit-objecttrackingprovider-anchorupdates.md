

- ARKit
- ObjectTrackingProvider
-  anchorUpdates 

Instance Property

# anchorUpdates

An asynchronous sequence of anchors the framework updates.

visionOS 2.0+

``` source
final var anchorUpdates: AnchorUpdateSequence { get }
```

## See Also

### Inspecting an object-tracking provider

var state: DataProviderState

The state of an object-tracking provider.

var allAnchors: [ObjectAnchor]

An array of all the object anchors the object-tracking provider is tracking.

struct Error

Values that represent an object-tracking error.

var description: String

A textual representation of this object tracking provider.

