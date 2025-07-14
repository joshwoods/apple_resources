

- ARKit
- HandTrackingProvider
-  latestAnchors 

Instance Property

# latestAnchors

The most recent hand anchors for each hand.

visionOS 1.0+

``` source
final var latestAnchors: (leftHand: HandAnchor?, rightHand: HandAnchor?) { get }
```

## Discussion

Accessing this tuple consumes its values and sets them to `nil` until the next anchor update. Both elements of this tuple are `nil` when the associated HandTrackingProvider isn’t running.

## See Also

### Observing hand anchor data

var anchorUpdates: AnchorUpdateSequence&lt;HandAnchor>

A sequence of updates for all hands that a provider tracks.

