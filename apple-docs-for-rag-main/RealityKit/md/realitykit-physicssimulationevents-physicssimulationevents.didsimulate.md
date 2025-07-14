

- RealityKit
- PhysicsSimulationEvents
-  PhysicsSimulationEvents.DidSimulate 

Structure

# PhysicsSimulationEvents.DidSimulate

The event raised after the simulation advances to the current frame.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct DidSimulate
```

## Topics

### Instance Properties

let deltaTime: TimeInterval

The time between last fixed update event and this one.

let simulationEntity: Entity

The root simulation entity associated with the simulation that raised the event.

## Relationships

### Conforms To

- Event
- Sendable

