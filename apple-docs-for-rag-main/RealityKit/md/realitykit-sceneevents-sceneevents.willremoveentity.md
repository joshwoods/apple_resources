

- RealityKit
- SceneEvents
-  SceneEvents.WillRemoveEntity 

Structure

# SceneEvents.WillRemoveEntity

Raised before an entity is removed from the scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct WillRemoveEntity
```

## Topics

### Instance Properties

let entity: Entity

## Relationships

### Conforms To

- Event
- Sendable

## See Also

### Detecting scene hierarchy changes

struct DidAddEntity

Raised after an entity is added to the scene.

struct DidReparentEntity

Raised after an entity has been reparented within the same scene.

struct DidActivateEntity

Raised after an entity becomes active.

struct WillDeactivateEntity

Raised before an entity becomes inactive.

