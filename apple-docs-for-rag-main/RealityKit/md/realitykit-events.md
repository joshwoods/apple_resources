

- RealityKit
-  Events 

API Collection

# Events

Respond to things happening in your RealityKit scene by subscribing to specific event types.

## Overview

You can receive notifications to specific RealityKit events — all of which conform to the Event protocol — by subscribing to specific events. The kinds of events you can subscribe to include the following:

- Two entities colliding

- An entity receiving a new component

- Audio playback reaching the end of its content

For example, you can receive a notification:

- When two objects begin colliding by subscribing to CollisionEvents.Began event

- When the scene redraws by subscribing to the SceneEvents.Update event

## Topics

### Core event types

protocol Event

A type that can be sent as an event.

protocol EventSource

A type on which events can be published and subscribed.

struct EventSubscription

A subscription to an event.

enum SceneEvents

Events the scene invokes.

enum ComponentEvents

Provides the events related to components.

### Physics and motion events

enum AnimationEvents

Notable milestones that the framework signals during animation playback.

enum CollisionEvents

enum PhysicsSimulationEvents

Types of events that fire during physics simulations

### Media events

enum AudioEvents

Events associated with audio playback.

enum VideoPlayerEvents

Events associated with video playback for VideoPlayerComponent.

### Accessibility events

enum AccessibilityEvents

### Network synchronization events

enum SynchronizationEvents

Events associated with network synchronization of scene information.

## See Also

### Scene management and logic

Scenes

The context that holds all RealityKit entities.

Systems

Apply behaviors and physical effects to the entities in a RealityKit scene.

Entity actions

Create simple, reusable actions that can change your app state, RealityKit scene, or animate an entity.

