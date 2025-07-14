

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  StartAnimationAction 

# StartAnimationAction

An action that plays an asset’s animation.

## Overview

If the asset defines an animation, this action runs it on every prim in affectedObjects.

### Declaration

```
class Preliminary_Action "StartAnimationAction"
```

## Topics

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

start

The moment to begin an animation.

duration

The amount of time that the objects face the camera.

reversed

A Boolean value that determines the clip playback direction.

animationSpeed

A factor to apply to the animation speed.

reverses

A Boolean value that indicates whether the animation plays from beginning to end, then again from end to beginning.

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

