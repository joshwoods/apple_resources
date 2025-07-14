

- RealityKit
- ComponentEvents
-  ComponentEvents.DidActivate 

Structure

# ComponentEvents.DidActivate

Event raised after a component has been activated.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct DidActivate
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

### Detecting component activations

struct WillDeactivate

Event raised before a component is deactivated.

