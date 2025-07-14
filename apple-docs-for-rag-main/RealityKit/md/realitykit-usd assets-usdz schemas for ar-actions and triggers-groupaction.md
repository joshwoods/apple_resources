

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  GroupAction 

# GroupAction

An action that runs a list of other actions.

## Overview

This action defines how the runtime executes each action in the actions array. When type is `serial`, the runtime performs actions one after the other. When type is `concurrent`, the runtime starts each action at the same time.

When this action’s type is `serial`, you can specify a delay between two actions by placing a `WaitAction` between them.

### Declaration

```
class Preliminary_Action "GroupAction"
```

### Create a sequential or looping group action

The following example defines a group of actions that run sequentially. The group contains a flip action, a wait action, and a hide action.

```
def Preliminary_Action "SimpleGroup" (
    inherits = 
)
{
    rel actions = [ , ,  ]
    uniform bool loops = false
    uniform uint performCount = 1

    def Action "Flip" (
        inherits = 
    )
    {
        uniform token motionType = "flip"
    }

    def Action "Wait" (
        inherits = 
    )
    {
    }

    def Action "Hide" (
        inherits = 
    )
    {
        uniform token type = "hide"
    }
}
```

The following group named `EndlessLoop` repeats a set of actions indefinitely because `performCount` is `0`.

```
def Action "EndlessLoop" (
    inherits = 
)
{
    rel actions = [...]
    uniform bool loops = true
    uniform uint performCount = 0
}
```

## Topics

### Properties

info:id

The action’s unique identifier.

type

An option that controls the order in which the actions execute.

loops

A Boolean value indicating whether the group loops.

performCount

A value that specifies the number of times the group’s actions repeat.

actions

A list of actions that make up the group.

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

