

- RealityKit
- CollisionEvents
-  CollisionEvents.Updated 

Structure

# CollisionEvents.Updated

An event raised on every frame when two objects are in contact.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct Updated
```

## Topics

### Getting the involved entities

let entityA: Entity

The first entity involved in the collision.

let entityB: Entity

The second entity involved in the collision.

### Characterizing the collision

let impulse: Float

The total impulse in this collision pair obtained by adding up all the individual impulses applied at each contact point

let position: SIMD3&lt;Float>

A position representing the estimated point of contact.

### Instance Properties

var contacts: [Contact]

All contacts between the collision pair. Empty if all contact information is not requested.

var impulseDirection: SIMD3&lt;Float>

The direction of the total impulse in scene coordinate space.

var penetrationDistance: Float

The estimated distance of overlap between the two colliding entities in scene coordinate space.

## Relationships

### Conforms To

- Event
- Sendable

## See Also

### Detecting collisions

struct Began

An event raised when two objects collide.

struct Ended

An event raised when two objects, previously in contact, separate.

