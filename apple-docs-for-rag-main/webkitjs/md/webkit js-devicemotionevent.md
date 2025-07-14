

- WebKit JS
-  DeviceMotionEvent 

Class

# DeviceMotionEvent

An instance of `DeviceMotionEvent` is created when significant change in motion occurs. The event object encapsulates the measurements of the interval, rotation rate, and acceleration of a device.

Safari Mobile 4.2+

``` source
interface DeviceMotionEvent
```

## Overview

The accelerometer measures the sum of two acceleration vectors: gravity and user acceleration. User acceleration is the acceleration that the user imparts to the device. Because the system is able to track the device’s attitude using both the gyroscope and the accelerometer, it can differentiate between gravity and user acceleration.

You register for these types of events using the window’s `addEventListener` method by passing `devicemotion` as the event type.

## Topics

### Creating Motion Events

initDeviceMotionEvent

Initializes a new device motion event.

### Getting Motion Event Properties

acceleration

The acceleration that the user is giving to the device.

accelerationIncludingGravity

The total acceleration of the device, which includes the user acceleration and the gravity.

interval

The interval in milliseconds since the last device motion event.

rotationRate

The rotation rate of the device.

## Relationships

### Inherits From

- Event

