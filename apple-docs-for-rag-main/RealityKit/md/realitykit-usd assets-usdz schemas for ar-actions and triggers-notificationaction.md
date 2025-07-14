

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  NotificationAction 

# NotificationAction

An action that sends a custom notification to an app.

## Overview

Use this action to perform an app-provided operation on a list of prims.

When this action executes, it posts a notification for which a custom app scans to perform a specific operation.

### Declaration

```
class Preliminary_Action "NotificationAction"
```

## Topics

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

identifier

A string value that identifies the app-specific notification.

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

VisibilityAction

An action that displays or hides objects over a period of time.

WaitAction

An action that performs a delay.

