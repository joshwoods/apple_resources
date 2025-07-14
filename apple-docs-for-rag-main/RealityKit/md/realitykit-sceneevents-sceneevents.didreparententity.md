

- RealityKit
- SceneEvents
-  SceneEvents.DidReparentEntity 

Structure

# SceneEvents.DidReparentEntity

Raised after an entity has been reparented within the same scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct DidReparentEntity
```

## Topics

### Instance Properties

let child: Entity

let previousParent: Entity?

## Relationships

### Conforms To

- Event
- Sendable

## See Also

### Detecting scene hierarchy changes

struct DidAddEntity

Raised after an entity is added to the scene.

struct WillRemoveEntity

Raised before an entity is removed from the scene.

struct DidActivateEntity

Raised after an entity becomes active.

struct WillDeactivateEntity

Raised before an entity becomes inactive.

