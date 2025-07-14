

- WebKit JS
- DeviceMotionEvent
-  initDeviceMotionEvent 

Instance Method

# initDeviceMotionEvent

Initializes a new device motion event.

Safari Mobile 4.2+

``` source
void initDeviceMotionEvent(
    optional DOMString type, 
    optional boolean bubbles, 
    optional boolean cancelable, 
    optional Acceleration acceleration, 
    optional Acceleration accelerationIncludingGravity, 
    optional RotationRate rotationRate, 
    optional unrestricted double interval
);
```

## Parameters 

`type`  

The type of event. Pass `devicemotion`.

`bubbles`  

Indicates whether this event is a bubbling event.

`cancelable`  

Indicates whether this event can be canceled.

`acceleration`  

The acceleration that the user is giving to the device. The `Acceleration` object has `x`, `y`, and `z` properties represented as doubles.

`accelerationIncludingGravity`  

The total acceleration of the device, which includes the user acceleration and the gravity. The `Acceleration` object has `x`, `y`, and `z` properties represented as doubles.

`rotationRate`  

The rotation rate of the device. The `RotationRate` object has `alpha`, `beta`, and `gamma` properties represented as doubles.

`interval`  

The interval in milliseconds since the last time this event was fired.

## See Also

### Related Documentation

Safari Web Content Guide

