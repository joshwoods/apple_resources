

- ARKit
- HandTrackingProvider
-  description 

Instance Property

# description

A textual representation of this hand tracking provider.

visionOS 1.0+

``` source
final var description: String { get }
```

## See Also

### Inspecting a hand-tracking provider

var state: DataProviderState

The current status of data coming from a provider.

func handAnchors(at: TimeInterval) -> (leftHand: HandAnchor?, rightHand: HandAnchor?)

Queries for hand anchors at the provided target timestamp.

