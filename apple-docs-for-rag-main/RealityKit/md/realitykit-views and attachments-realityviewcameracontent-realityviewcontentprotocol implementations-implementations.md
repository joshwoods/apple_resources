

- RealityKit
- Views and attachments
- RealityViewCameraContent
-  RealityViewContentProtocol Implementations 

API Collection

# RealityViewContentProtocol Implementations

## Topics

### Instance Methods

func add(Entity)

Adds an entity to this content.

func remove(Entity)

Removes an entity from this content, if present.

func subscribe&lt;E>(to: E.Type, componentType: (any Component.Type)?, (E) -> Void) -> EventSubscription

Subscribes to an event type, optionally limited to a specific component type for component events.

func subscribe&lt;E>(to: E.Type, on: (any EventSource)?, (E) -> Void) -> EventSubscription

Subscribes to an event type, optionally limited to events affecting a source entity or scene.

