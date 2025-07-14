

- RealityKit
-  Entity actions 

API Collection

# Entity actions

Create simple, reusable actions that can change your app state, RealityKit scene, or animate an entity.

## Overview

Entity actions provide an easy way to change or animate parts of your scene, while also allowing you to influence the changes with your app state.

For example, you can vary the size of an impulse you apply to an entity with ImpulseAction, play a sound at the end of an entity’s animation with PlayAudioAction, or create a custom action that changes your app state.

## Topics

### Action management

protocol EntityAction

A protocol that defines an action for an entity.

struct ActionAnimation

Defines an an action animation.

enum ActionEntityResolution

Options available to determine the resolution method for a target entity in an action.

protocol ActionHandlerProtocol

The base protocol for action handlers.

### Action events

struct ActionEvent

The structure returned to all action event handlers.

struct AnimationState

The concretely typed animation state structure.

struct ActionEventType

A set of events that an action responds to.

struct ActionEventDefinition

Defines an action event interval, and any associated parameters.

protocol AnimationStateProtocol

The protocol representing the current animation state of an action animation.

### Built-in actions

struct BillboardAction

An action that animates the blend factor of an entity’s billboard component.

struct EmphasizeAction

An action that performs an animation to call attention to an entity.

struct FromToByAction

An action that starts, stops, or increments by a specific value.

struct ImpulseAction

An action that applies an impulse to the physics body at its center of mass when played as an animation.

struct OrbitEntityAction

An action which animates the transform of an entity to revolve around a specified pivot entity.

struct PlayAnimationAction

An action that plays an animation on the given target entity with a range of playback options.

struct PlayAudioAction

An action which plays an audio resource on the given target entity.

struct SetEntityEnabledAction

An action that enables or disables the targeted entity and its descendants when played as an animation.

struct SpinAction

An action which animates the transform of an entity to rotate around a specified local axis.

## See Also

### Scene management and logic

Scenes

The context that holds all RealityKit entities.

Systems

Apply behaviors and physical effects to the entities in a RealityKit scene.

Events

Respond to things happening in your RealityKit scene by subscribing to specific event types.

