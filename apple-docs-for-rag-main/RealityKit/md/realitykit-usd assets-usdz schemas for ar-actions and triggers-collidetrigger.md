

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  CollideTrigger 

# CollideTrigger

A trigger that activates when specified objects collide.

## Overview

The runtime fires this trigger when any of the prims in the list of affectedObjects collide with any of the prims in colliders.

If all objects can collide with each other, define affectedObjects and colliders as the same list.

### Declaration

```
class Preliminary_Trigger "CollideTrigger"
```

## Topics

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

colliders

A list of prims that interact with objects to create a collision.

## See Also

### Triggers

Preliminary_Trigger

A condition that, when met, performs an action.

ProximityToCameraTrigger

A trigger that fires when the camera crosses the distance threshold of an object.

SceneTransitionTrigger

A trigger that fires during scene transitions.

TapGestureTrigger

A trigger that fires when the user taps.

NotificationTrigger

A trigger that fires when an app posts a notification.

