

- ARKit
- HandTrackingProvider
-  anchorUpdates 

Instance Property

# anchorUpdates

A sequence of updates for all hands that a provider tracks.

visionOS 1.0+

``` source
final var anchorUpdates: AnchorUpdateSequence { get }
```

## See Also

### Observing hand anchor data

var latestAnchors: (leftHand: HandAnchor?, rightHand: HandAnchor?)

The most recent hand anchors for each hand.

