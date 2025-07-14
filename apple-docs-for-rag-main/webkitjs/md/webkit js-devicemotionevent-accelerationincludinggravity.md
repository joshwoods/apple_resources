

- WebKit JS
- DeviceMotionEvent
-  accelerationIncludingGravity 

Instance Property

# accelerationIncludingGravity

The total acceleration of the device, which includes the user acceleration and the gravity.

Safari Mobile 4.2+

``` source
readonly attribute Acceleration accelerationIncludingGravity;
```

## Discussion

The acceleration data is expressed in m/s^2 and use the `x`, `y`, and `z` axis properties described in acceleration. This property is never `null` because every Apple device has an accelerometer.

Use the `acceleration` property to get the user acceleration only.

## See Also

### Getting Motion Event Properties

acceleration

The acceleration that the user is giving to the device.

interval

The interval in milliseconds since the last device motion event.

rotationRate

The rotation rate of the device.

