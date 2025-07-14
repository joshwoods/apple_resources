

- ARKit
- HandTrackingProvider
-  handAnchors(at:) 

Instance Method

# handAnchors(at:)

Queries for hand anchors at the provided target timestamp.

visionOS 2.0+

``` source
final func handAnchors(at timestamp: TimeInterval) -> (leftHand: HandAnchor?, rightHand: HandAnchor?)
```

## Parameters 

`timestamp`  

The target timestamp, mach absolute time, in seconds.

## Return Value

A tuple that contains optional left and right anchors for the given time. Anchors are `nil` when the provider isn’t running.

## Discussion

Important

This function isn’t safe to call on multiple threads at the same time. You need to provide your own synchronization.

## See Also

### Inspecting a hand-tracking provider

var state: DataProviderState

The current status of data coming from a provider.

var description: String

A textual representation of this hand tracking provider.

