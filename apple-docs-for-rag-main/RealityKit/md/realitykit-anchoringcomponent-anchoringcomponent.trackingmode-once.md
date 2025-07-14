

- RealityKit
- AnchoringComponent
- AnchoringComponent.TrackingMode
-  once 

Type Property

# once

Anchors the entity to the target on the first frame the target is found.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
static let once: AnchoringComponent.TrackingMode
```

## Discussion

`once` means the `Entity` transform is evaluated only once when the target anchor presents and the `Entity` is anchored.

If the target anchor moves or disappears later, the `Entity` stays in place.

