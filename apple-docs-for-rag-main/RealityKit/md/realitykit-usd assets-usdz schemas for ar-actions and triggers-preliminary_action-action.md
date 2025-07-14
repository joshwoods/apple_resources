

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  Preliminary_Action 

# Preliminary_Action

A specific task that a trigger performs.

## Overview

Because it inherits `Typed`, this schema declares a `Preliminary_Action` as a type of prim. For more information about typed schemas, see USD Specification \> Typed.

When a behavior executes an action, the behavior modifies the state of the scene dynamically. For example, an action might start an animation, change the location of a prim, or start playing audio.

### Declaration

```
class "Preliminary_Action" (
    inherits = 
)
```

### Define an action that slides a cube

The following example shows an action prim called `PushCube` that affects an impulse feature.

```
#usda 1.0

def Cube "Cube" {}

def Preliminary_Action "PushCube" {    
    uniform token info:id = "Impulse"
    rel affectedObjects = [  ]
    uniform vector3d velocity = (1.0, 0.0, 0.0)
}
```

## Topics

### Properties

info:id

The action’s unique identifier.

multiplePerformOperation

An option that indicates how an action handles an additional invocation while running.

## See Also

### Actions

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

