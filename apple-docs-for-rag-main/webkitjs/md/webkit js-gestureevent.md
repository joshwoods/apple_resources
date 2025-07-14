

- WebKit JS
-  GestureEvent 

Class

# GestureEvent

The `GestureEvent` class encapsulates information about a multi-touch gesture.

Safari Desktop 10.1+Safari Mobile 2.0+

``` source
interface GestureEvent
```

## Overview

`GestureEvent` objects are high-level events that encapsulate the low-level TouchEvent objects. Both `GestureEvent` and `TouchEvent` events are sent during a multi-touch sequence. Gesture events contain scaling and rotation information allowing gestures to be combined, if supported by the platform. If not supported, one gesture ends before another starts. Listen for `GestureEvent` events if you want to respond to gestures only, not process the low-level `TouchEvent` objects.

The different types of `GestureEvent` objects that can occur are:

`gesturestart`  
Sent when two or more fingers touch the surface.

`gesturechange`  
Sent when fingers are moved during a gesture.

`gestureend`  
Sent when the gesture ends (when there are 1 or 0 fingers touching the surface).

For example, for a two finger multi-touch gesture, the events occur in the following sequence:

1.  `touchstart` for finger 1. Sent when the first finger touches the surface.

2.  `gesturestart`. Sent when the second finger touches the surface.

3.  `touchstart` for finger 2. Sent immediately after `gesturestart` when the second finger touches the surface.

4.  `gesturechange` for current gesture. Sent when both fingers move while still touching the surface.

5.  `gestureend`. Sent when the second finger lifts from the surface.

6.  `touchend` for finger 2. Sent immediately after `gestureend` when the second finger lifts from the surface.

7.  `touchend` for finger 1. Sent when the first finger lifts from the surface.

See TouchEvent if you want to process just low-level `TouchEvent` objects.

## Topics

### Accessing Properties

altKey

A Boolean value indicating whether the alt key is pressed.

ctrlKey

A Boolean value indicating whether the control key is pressed.

metaKey

A Boolean value indicating whether the meta key is pressed.

rotation

The delta rotation since the start of an event, in degrees, where clockwise is positive and counter-clockwise is negative.

scale

The distance between two fingers since the start of an event, as a multiplier of the initial distance.

shiftKey

A Boolean value indicating whether the shift key is pressed.

target

The target of this gesture.

### Initializing

initGestureEvent

Initializes a newly created `GestureEvent` object.

### Instance Properties

clientX

clientY

screenX

screenY

## Relationships

### Inherits From

- UIEvent

