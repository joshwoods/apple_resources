

- RealityKit
- USD Assets
- USDZ schemas for AR
-  Actions and triggers 

# Actions and triggers

Enable visual and audible responses to programmatic or environmental events.

## Overview

Create a `Preliminary_Behavior` to uniquely pair triggers with actions. You can configure some of the triggers and actions, like the settings for a proximity trigger, the velocity of an impulse action, and the audio file for background music or sound effects.

The runtime implements the concrete triggers and actions the schemas define. The exception is `NotificationAction`, which refers to custom effects that an app implements.

## Topics

### Essentials

Preliminary_Behavior

A typed schema that combines one or more triggers with associated actions.

### Triggers

Control when the runtime executes an action.

Preliminary_Trigger

A condition that, when met, performs an action.

CollideTrigger

A trigger that activates when specified objects collide.

ProximityToCameraTrigger

A trigger that fires when the camera crosses the distance threshold of an object.

SceneTransitionTrigger

A trigger that fires during scene transitions.

TapGestureTrigger

A trigger that fires when the user taps.

NotificationTrigger

A trigger that fires when an app posts a notification.

### Actions

Execute a unique response to a trigger.

Preliminary_Action

A specific task that a trigger performs.

AudioAction

An action that plays audio.

ChangeSceneAction

An action that transitions from one scene to another.

EmphasizeAction

An action that performs an animation to call attention to an object.

GroupAction

An action that runs a list of other actions.

ImpulseAction

An action that adds velocity to an prim.

LookAtCameraAction

An action that reorients an object to face the user’s camera.

OrbitAction

An action that orbits a set of prims around another.

SpinAction

An action that spins a prim.

StartAnimationAction

An action that plays an asset’s animation.

TransformAction

An action that animates from one transform to another.

TransformAnimationAction

An action that plays a transform animation.

VisibilityAction

An action that displays or hides objects over a period of time.

WaitAction

An action that performs a delay.

NotificationAction

An action that sends a custom notification to an app.

