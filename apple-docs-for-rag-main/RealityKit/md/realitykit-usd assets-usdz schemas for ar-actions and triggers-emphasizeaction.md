

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  EmphasizeAction 

# EmphasizeAction

An action that performs an animation to call attention to an object.

## Overview

Instead of specifying your own animation, choose from the preexisting options in motionType.

### Declaration

```
class Preliminary_Action "EmphasizeAction"
```

## Topics

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

duration

The amount of time that the objects face the camera.

style

An option that implements different kinds of animation timing.

motionType

An option that determines how the action displays or hides a prim.

## See Also

### Actions

Preliminary_Action

A specific task that a trigger performs.

AudioAction

An action that plays audio.

ChangeSceneAction

An action that transitions from one scene to another.

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

