

- WebKit JS
-  Touch 

Class

# Touch

A `Touch` object represents a single user touch on the screen of the device. A touch is the presence or movement of a finger and is part of a unique multi-touch sequence. Use the changedTouches method to get all the touch objects that changed in a TouchEvent object.

Safari Desktop 10.1+Safari Mobile 2.0+

``` source
interface Touch
```

## Overview

Starting in iOS 9, on devices that support 3D Touch, you can get the force property of the `Touch` class to obtain a value representing the force at which the user is pressing on the screen. For more information about 3D Touch, see *Adopting 3D Touch on iPhone*.

## Topics

### Accessing Properties

target

The target of this touch.

identifier

The unique identifier for this touch object.

clientX

The x-coordinate of the touch’s location relative to the window’s viewport.

clientY

The y-coordinate of the touch’s location relative to the window’s viewport.

pageX

The x-coordinate of the touch’s location in page coordinates.

pageY

The y-coordinate of the touch’s location in page coordinates.

screenX

The x-coordinate of the touch’s location in screen coordinates.

screenY

The y-coordinate of the touch’s location in screen coordinates.

force

The force of the touch, using a positive linear scale where a value of `0.0` indicates the absence of force.

### Instance Properties

altitudeAngle

azimuthAngle

radiusX

radiusY

rotationAngle

touchType

