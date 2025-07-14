

- RealityKit
- SceneEvents
-  SceneEvents.DidAddEntity 

Structure

# SceneEvents.DidAddEntity

Raised after an entity is added to the scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct DidAddEntity
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

struct DidReparentEntity

Raised after an entity has been reparented within the same scene.

struct WillRemoveEntity

Raised before an entity is removed from the scene.

struct DidActivateEntity

Raised after an entity becomes active.

struct WillDeactivateEntity

Raised before an entity becomes inactive.

