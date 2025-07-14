

- RealityKit
- ComponentEvents
-  ComponentEvents.DidAdd 

Structure

# ComponentEvents.DidAdd

Event raised after a component has been added to an entity,

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct DidAdd
```

## Topics

### Instance Properties

let componentType: any Component.Type

The component type.

let entity: Entity

The component’s entity.

## Relationships

### Conforms To

- Event
- Sendable

## See Also

### Detecting component changes

struct DidChange

Event raised after a component has been modified.

struct WillRemove

Event raised before a component is removed from an entity.

