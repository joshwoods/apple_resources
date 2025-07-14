

- RealityKit
-  Event 

Protocol

# Event

A type that can be sent as an event.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
protocol Event : Sendable
```

## Overview

RealityKit provides a number of events you can subscribe to. The system notifies you whenever the event type occurs.

For example, you can subscribe to CollisionEvents.Began to know when two objects begin colliding, or SceneEvents.Update every time the scene redraws.

To subscribe to an event from inside of a RealityView builder, call one of the RealityViewContentProtocol `subscribe` methods, for example subscribe(to:on:_:).

Here’s an example of subscribing to the event CollisionEvents.Began, which occurs when two entities collide:

```
struct RealityGame: View {

    @State var collisionSubscription: EventSubscription?

    var body: some View {
        RealityView { content in
            // Create an entity with model and collision components.
            let model = ModelComponent(
                mesh: MeshResource.generateBox(size: .one / 10),
                materials: [SimpleMaterial(color: .red, isMetallic: false)]
            )
            let collision = CollisionComponent(shapes: [ShapeResource.generateBox(size: .one / 10)])
            let collisionEntity = Entity(components: model, collision)
            content.add(collisionEntity)

            // Subscribe to collision began event.
            collisionSubscription = content.subscribe(
               to: CollisionEvents.Began.self,
               on: collisionEntity,
               self.onCollisionBegan
           )
        }
    }
    private func onCollisionBegan(_ event: CollisionEvents.Began) {
        print("collision started")
        let firstEntity = event.entityA // The entity whose collisions you're subscribing to.
        let secondEntity = event.entityB // Another entity in the scene.
        // Respond to collision event...
    }
}
```

Note

Add a CollisionComponent to any entities you want to detect collisions for.

## Relationships

### Inherits From

- Sendable

### Conforming Types

- AccessibilityEvents.Activate
- AccessibilityEvents.CustomAction
- AccessibilityEvents.Decrement
- AccessibilityEvents.Increment
- AccessibilityEvents.RotorNavigation
- AnimationEvents.PlaybackCompleted
- AnimationEvents.PlaybackLooped
- AnimationEvents.PlaybackStarted
- AnimationEvents.PlaybackTerminated
- AnimationEvents.SkeletalPoseUpdateComplete
- AudioEvents.PlaybackCompleted
- CollisionEvents.Began
- CollisionEvents.Ended
- CollisionEvents.Updated
- ComponentEvents.DidActivate
- ComponentEvents.DidAdd
- ComponentEvents.DidChange
- ComponentEvents.WillDeactivate
- ComponentEvents.WillRemove
- PhysicsSimulationEvents.DidSimulate
- PhysicsSimulationEvents.WillSimulate
- SceneEvents.AnchoredStateChanged
- SceneEvents.DidActivateEntity
- SceneEvents.DidAddEntity
- SceneEvents.DidReparentEntity
- SceneEvents.Update
- SceneEvents.WillDeactivateEntity
- SceneEvents.WillRemoveEntity
- SynchronizationEvents.OwnershipChanged
- SynchronizationEvents.OwnershipRequest
- VideoPlayerEvents.ContentTypeDidChange
- VideoPlayerEvents.ImmersiveViewingModeDidChange
- VideoPlayerEvents.ImmersiveViewingModeDidTransition
- VideoPlayerEvents.ImmersiveViewingModeWillTransition
- VideoPlayerEvents.VideoSizeDidChange
- VideoPlayerEvents.ViewingModeDidChange

## See Also

### Core event types

protocol EventSource

A type on which events can be published and subscribed.

struct EventSubscription

A subscription to an event.

enum SceneEvents

Events the scene invokes.

enum ComponentEvents

Provides the events related to components.

