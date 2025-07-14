

- WebKit JS
-  TouchEvent 

Class

# TouchEvent

The `TouchEvent` class encapsulates information about a touch event.

Safari Desktop 10.1+Safari Mobile 2.0+

``` source
interface TouchEvent
```

## Overview

The system continually sends `TouchEvent` objects to an application as fingers touch and move across a surface. A touch event provides a snapshot of all touches during a multi-touch sequence, most importantly the touches that are new or have changed for a particular target. A multi-touch sequence begins when a finger first touches the surface. Other fingers may subsequently touch the surface, and all fingers may move across the surface. The sequence ends when the last of these fingers is lifted from the surface. An application receives touch event objects during each phase of any touch.

The different types of `TouchEvent` objects that can occur are:

`touchstart`  
Sent when a finger for a given event touches the surface.

`touchmove`  
Sent when a given event moves on the surface.

`touchend`  
Sent when a given event lifts from the surface.

`touchcancel`  
Sent when the system cancels tracking for the touch.

`TouchEvent` objects are combined together to form high-level `GestureEvent` objects that are also sent during a multi-touch sequence. See GestureEvent for details on `GestureEvent` objects and an example of the events sent for a two finger multi-touch gesture.

## Topics

### Accessing Properties

altKey

A Boolean value indicating whether the alt key is pressed.

ctrlKey

A Boolean value indicating whether the control key is pressed.

metaKey

A Boolean value indicating whether the meta key is pressed.

shiftKey

A Boolean value indicating whether the shift key is pressed.

changedTouches

A collection of Touch objects representing all touches that changed in this event.

targetTouches

A collection of Touch objects representing all touches associated with this target.

touches

A collection of Touch objects representing all touches associated with this event.

rotation

The delta rotation since the start of an event in degrees where clockwise is positive and counter-clockwise is negative.

scale

The distance between two fingers since the start of an event as a multiplier of the initial distance.

### Initializing

initTouchEvent

Initializes a newly created `TouchEvent` object.

## Relationships

### Inherits From

- UIEvent

