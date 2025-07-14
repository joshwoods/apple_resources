

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  Preliminary_Behavior 

# Preliminary_Behavior

A typed schema that combines one or more triggers with associated actions.

## Overview

Because it inherits `Typed`, this schema declares a `Preliminary_Behavior` as a type of prim. For more information about typed schemas, see USD Specification \> Typed.

To run actions based on a trigger, an asset defines a prim of this type and sets its triggers and actions.

### Declaration

```
class Preliminary_Behavior "Preliminary_Behavior" (
    inherits = 
)
```

### Trigger animation for a tapped cube

The following example demonstrates a behavior that applies an `EmphasizeAction` to a cube to flip it. Because the cube defines a tap trigger, the runtime performs the flip when a user taps the cube in an AR experience.

```
#usda 1.0

def Preliminary_Behavior "TapAndFlip"
{
    rel triggers = [  ]
    rel actions = [  ]

    def Preliminary_Trigger "Tap" ( inherits =  )
    {
        rel affectedObjects = [  ]
    }

    def Preliminary_Action "Entry" ( inherits =  )
    {
        uniform token type = "parallel"
        rel actions = [  ]
    }

    def Preliminary_Action "Flip" ( inherits =  )
    {
        rel affectedObjects = [  ]
        uniform token motionType = "flip"
    }
}

def Cube "Cube" { }
```

## Topics

### Properties

triggers

A list of prims that execute a behavior’s actions.

actions

A list of actions that make up the group.

exclusive

A Boolean value that determines if a behavior executes exclusively.

