

- WebKit JS
-  DeviceOrientationEvent 

Class

# DeviceOrientationEvent

Instances of the `DeviceOrientationEvent` class are fired only when the device has a gyroscope and while the user is changing the orientation. The `DeviceOrientationEvent` class encapsulates the angles of rotation in degrees and heading.

Safari Mobile 4.2+

``` source
interface DeviceOrientationEvent
```

## Overview

The angles of rotation—the alpha, beta, and gamma properties—do not represent the real world orientation. They are defined as an offset from an arbitrary direction—typically, the direction in which the device was held when the orientation was first obtained. Therefore, you can only use the angles to track changes in orientation, you cannot derive the direction in which the device is currently facing. To track changes, save the first device orientation event and use it as a reference for subsequent values. If you want a real world heading, use the webkitCompassHeading property.

Because some devices may not have a gyroscope, you can listen for this event. If it does not occur, use the DeviceMotionEvent class to receive raw accelerometer events. From these events you can determine an approximate orientation.

You register for device orientation events using the window’s `addEventListener` method by passing `deviceorientation` as the event type.

## Topics

### Creating Orientation Events

initDeviceOrientationEvent

Initializes a new device orientation event.

### Getting Orientation Event Properties

alpha

The rotation, in degrees, of the device frame around its z-axis.

beta

The rotation, in degrees, of the device frame around its x-axis.

gamma

The rotation, in degrees, of the device frame around its y-axis.

### Getting Compass Properties

webkitCompassAccuracy

The accuracy of the compass data in degrees.

webkitCompassHeading

A direction that is measured in degrees relative to magnetic north.

### Instance Properties

absolute

## Relationships

### Inherits From

- Event

