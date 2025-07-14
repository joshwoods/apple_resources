

- ARKit
- HandTrackingProvider
-  state 

Instance Property

# state

The current status of data coming from a provider.

visionOS 1.0+

``` source
final var state: DataProviderState { get }
```

## See Also

### Inspecting a hand-tracking provider

var description: String

A textual representation of this hand tracking provider.

func handAnchors(at: TimeInterval) -> (leftHand: HandAnchor?, rightHand: HandAnchor?)

Queries for hand anchors at the provided target timestamp.

