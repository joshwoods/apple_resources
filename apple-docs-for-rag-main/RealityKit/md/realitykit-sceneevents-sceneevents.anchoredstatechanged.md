

- RealityKit
- SceneEvents
-  SceneEvents.AnchoredStateChanged 

Structure

# SceneEvents.AnchoredStateChanged

An event invoked when the anchored state of an anchoring entity changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct AnchoredStateChanged
```

## Topics

### Characterizing an update

let anchor: any HasAnchoring

The entity whose anchoring state changed.

let isAnchored: Bool

The current anchoring state of the entity.

## Relationships

### Conforms To

- Event
- Sendable

## See Also

### Detecting scene-level updates

struct Update

An event invoked once per frame interval that you can use to execute custom logic for each frame.

