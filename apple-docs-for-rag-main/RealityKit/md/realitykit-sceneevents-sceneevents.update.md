

- RealityKit
- SceneEvents
-  SceneEvents.Update 

Structure

# SceneEvents.Update

An event invoked once per frame interval that you can use to execute custom logic for each frame.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct Update
```

## Topics

### Characterizing an update

let scene: Scene

The updated scene.

let deltaTime: TimeInterval

The elapsed time since the last update.

## Relationships

### Conforms To

- Event
- Sendable

## See Also

### Detecting scene-level updates

struct AnchoredStateChanged

An event invoked when the anchored state of an anchoring entity changes.

