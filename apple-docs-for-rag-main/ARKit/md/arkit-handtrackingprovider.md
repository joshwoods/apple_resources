

- ARKit
-  HandTrackingProvider 

Class

# HandTrackingProvider

A source of live data about the position of a person’s hands and hand joints.

visionOS 1.0+

``` source
final class HandTrackingProvider
```

## Topics

### Creating a hand-tracking provider

init()

Creates a hand-tracking provider.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports hand-tracking providers.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The types of authorizations necessary for tracking hands.

### Observing hand anchor data

var anchorUpdates: AnchorUpdateSequence&lt;HandAnchor>

A sequence of updates for all hands that a provider tracks.

var latestAnchors: (leftHand: HandAnchor?, rightHand: HandAnchor?)

The most recent hand anchors for each hand.

### Inspecting a hand-tracking provider

var state: DataProviderState

The current status of data coming from a provider.

var description: String

A textual representation of this hand tracking provider.

func handAnchors(at: TimeInterval) -> (leftHand: HandAnchor?, rightHand: HandAnchor?)

Queries for hand anchors at the provided target timestamp.

## Relationships

### Conforms To

- CustomStringConvertible
- DataProvider
- Sendable

## See Also

### Hand tracking

Happy Beam

Leverage a Full Space to create a fun game using ARKit.

struct HandAnchor

A hand’s position in a person’s surroundings.

struct HandSkeleton

A collection of joints in a hand.

