

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  VisibilityAction 

# VisibilityAction

An action that displays or hides objects over a period of time.

## Overview

Use this action to display or hide a prim with a transform animation. This action is distinct from `UsdGeomImageable` because the animation doesn’t alter the `visible` property.

### Declaration

```
class Preliminary_Action "VisibilityAction"
```

## Topics

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

type

An option that controls the order in which the actions execute.

style

An option that implements different kinds of animation timing.

motionType

An option that determines how the action displays or hides a prim.

easeType

An option that describes the animation’s change in pace over time.

moveDistance

The distance that this action moves the target prims.

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

TransformAction

An action that animates from one transform to another.

TransformAnimationAction

An action that plays a transform animation.

WaitAction

An action that performs a delay.

NotificationAction

An action that sends a custom notification to an app.

