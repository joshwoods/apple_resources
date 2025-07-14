

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  ChangeSceneAction 

# ChangeSceneAction

An action that transitions from one scene to another.

## Overview

To define multiple scenes in a USDZ file, use the `def` and `over` specifiers. For more information, see sceneLibrary.

### Declaration

```
class Preliminary_Action "ChangeSceneAction"
```

## Topics

### Properties

info:id

The action’s unique identifier.

scene

The scene to which the action transitions.

## See Also

### Actions

Preliminary_Action

A specific task that a trigger performs.

AudioAction

An action that plays audio.

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

