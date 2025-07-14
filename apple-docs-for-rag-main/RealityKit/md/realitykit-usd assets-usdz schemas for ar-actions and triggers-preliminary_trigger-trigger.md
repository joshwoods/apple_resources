

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  Preliminary_Trigger 

# Preliminary_Trigger

A condition that, when met, performs an action.

## Overview

Because it inherits `Typed`, this schema declares a `Preliminary_Trigger` as a type of prim. For more information about typed schemas, see USD Specification \> Typed.

The runtime executes triggers based on:

- User input, like a user’s tap gesture.

- Scene state, including a prim’s proximity to the user’s device.

- Programmatic conditions, like application state or a function result.

### Declaration

```
class "Preliminary_Trigger" (
    inherits = 
)
```

### Add a tap trigger to a cube

The following example shows how a prim named `TapCube` opts in to notification of user taps.

```
#usda 1.0

def Cube "Cube" {}

def Preliminary_Trigger "TapCube" {
    uniform token info:id = "TapGesture"
    rel affectedObjects = [  ]
}
```

## Topics

### Properties

info:id

The action’s unique identifier.

## See Also

### Triggers

CollideTrigger

A trigger that activates when specified objects collide.

ProximityToCameraTrigger

A trigger that fires when the camera crosses the distance threshold of an object.

SceneTransitionTrigger

A trigger that fires during scene transitions.

TapGestureTrigger

A trigger that fires when the user taps.

NotificationTrigger

A trigger that fires when an app posts a notification.

