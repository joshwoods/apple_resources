

- RealityKit
- CollisionEvents
-  CollisionEvents.Ended 

Structure

# CollisionEvents.Ended

An event raised when two objects, previously in contact, separate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct Ended
```

## Topics

### Getting the involved entities

let entityA: Entity

The first entity involved in the collision.

let entityB: Entity

The second entity involved in the collision.

## Relationships

### Conforms To

- Event
- Sendable

## See Also

### Detecting collisions

struct Began

An event raised when two objects collide.

struct Updated

An event raised on every frame when two objects are in contact.

