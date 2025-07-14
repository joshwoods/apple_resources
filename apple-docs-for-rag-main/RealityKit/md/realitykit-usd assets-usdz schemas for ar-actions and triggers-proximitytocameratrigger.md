

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  ProximityToCameraTrigger 

# ProximityToCameraTrigger

A trigger that fires when the camera crosses the distance threshold of an object.

## Overview

The runtime fires this trigger one time when the distance threshold it specifies is met. The runtime can fire the trigger again only if the user moves away from the threshold and then returns.

### Declaration

```
class Preliminary_Trigger "ProximityToCameraTrigger"
```

## Topics

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

distance

A threshold that measures the user’s proximity to one or more prims.

## See Also

### Triggers

Preliminary_Trigger

A condition that, when met, performs an action.

CollideTrigger

A trigger that activates when specified objects collide.

SceneTransitionTrigger

A trigger that fires during scene transitions.

TapGestureTrigger

A trigger that fires when the user taps.

NotificationTrigger

A trigger that fires when an app posts a notification.

