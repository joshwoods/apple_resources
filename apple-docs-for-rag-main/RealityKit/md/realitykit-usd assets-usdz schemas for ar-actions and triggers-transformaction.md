

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  TransformAction 

# TransformAction

An action that animates from one transform to another.

## Overview

This action animates from the target prim’s current transform to the xformTarget transform.

### Declaration

```
class Preliminary_Action "TransformAction"
```

## Topics

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

xformTarget

A prim that provides the transform to which this action animates.

duration

The amount of time that the objects face the camera.

type

An option that controls the order in which the actions execute.

easeType

An option that describes the animation’s change in pace over time.

## See Also

### Actions

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

TransformAnimationAction

An action that plays a transform animation.

VisibilityAction

An action that displays or hides objects over a period of time.

WaitAction

An action that performs a delay.

NotificationAction

An action that sends a custom notification to an app.

