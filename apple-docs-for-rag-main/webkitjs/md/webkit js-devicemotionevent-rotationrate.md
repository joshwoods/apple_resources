

- WebKit JS
- DeviceMotionEvent
-  rotationRate 

Instance Property

# rotationRate

The rotation rate of the device.

Safari Mobile 4.2+

``` source
readonly attribute RotationRate rotationRate;
```

## Discussion

The `RotationRate` object specifies the device’s rate of rotation around three axes. It contains `alpha`, `beta`, and `gamma` properties represented as doubles as described in DeviceOrientationEvent.

This property is `null` if the device cannot provide the rate of rotation—that is, if the device does not have a gyroscope.

## See Also

### Getting Motion Event Properties

acceleration

The acceleration that the user is giving to the device.

accelerationIncludingGravity

The total acceleration of the device, which includes the user acceleration and the gravity.

interval

The interval in milliseconds since the last device motion event.

