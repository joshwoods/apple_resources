

- ARKit
- ObjectTrackingProvider
-  state 

Instance Property

# state

The state of an object-tracking provider.

visionOS 2.0+

``` source
final var state: DataProviderState { get }
```

## See Also

### Inspecting an object-tracking provider

var allAnchors: [ObjectAnchor]

An array of all the object anchors the object-tracking provider is tracking.

var anchorUpdates: AnchorUpdateSequence&lt;ObjectAnchor>

An asynchronous sequence of anchors the framework updates.

struct Error

Values that represent an object-tracking error.

var description: String

A textual representation of this object tracking provider.

