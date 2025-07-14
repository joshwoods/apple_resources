

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  OrbitAction 

# OrbitAction

An action that orbits a set of prims around another.

## Overview

This action sends the list of prims defined by affectedObjects into orbit at a fixed distance around its center prim, on a plane perpendicular to the axis of rotation. The runtime caculates the fixed distance as a straight line between the respective origins of the affectedObjects and the center.

### Declaration

```
class Preliminary_Action "OrbitAction"
```

## Topics

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

center

A prim around which the affected objects orbit.

duration

The amount of time that the objects face the camera.

revolutions

The number of rotations to complete.

axis

A vector that describes the axis of rotation.

alignToPath

An option that controls the prim’s orientation as it revolves.

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

