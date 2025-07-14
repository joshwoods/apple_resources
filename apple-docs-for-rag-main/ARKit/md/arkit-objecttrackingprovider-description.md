

- ARKit
- ObjectTrackingProvider
-  description 

Instance Property

# description

A textual representation of this object tracking provider.

visionOS 2.0+

``` source
final var description: String { get }
```

## See Also

### Inspecting an object-tracking provider

var state: DataProviderState

The state of an object-tracking provider.

var allAnchors: [ObjectAnchor]

An array of all the object anchors the object-tracking provider is tracking.

var anchorUpdates: AnchorUpdateSequence&lt;ObjectAnchor>

An asynchronous sequence of anchors the framework updates.

struct Error

Values that represent an object-tracking error.

