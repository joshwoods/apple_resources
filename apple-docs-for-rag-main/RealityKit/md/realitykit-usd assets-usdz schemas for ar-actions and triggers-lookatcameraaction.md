

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  LookAtCameraAction 

# LookAtCameraAction

An action that reorients an object to face the user’s camera.

## Overview

By default, the duration specifies the amount of time the prim looks at the camera. To look at the camera indefinitely, place this action in a `GroupAction` that repeats infinitely.

### Declaration

```
class Preliminary_Action "LookAtCameraAction"
```

## Topics

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

duration

The amount of time that the objects face the camera.

front

A vector that’s perpendicular to, and points outward from, the object’s face.

upVector

A vector around which the runtime rotates the object.

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

