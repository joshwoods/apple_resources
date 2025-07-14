

- RealityKit
- AnchoringComponent
- AnchoringComponent.TrackingMode
-  continuous 

Type Property

# continuous

Continuously anchors the entity to its target based on the target’s realtime location and hides the entity when the target is no longer in frame.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
static let continuous: AnchoringComponent.TrackingMode
```

## Discussion

`continuous` means the `Entity` will track the target anchor continuously.

The `Entity` moves with the anchor and is unanchored if the target anchor disappears or no longer meets the target requirement.

