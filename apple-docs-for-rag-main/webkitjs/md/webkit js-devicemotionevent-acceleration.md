

- WebKit JS
- DeviceMotionEvent
-  acceleration 

Instance Property

# acceleration

The acceleration that the user is giving to the device.

Safari Mobile 4.2+

``` source
readonly attribute Acceleration acceleration;
```

## Discussion

The acceleration data are expressed in m/s^2 and use the following `x`, `y`, and `z` axis properties represented as doubles:

x  
In the plane of the screen, positive towards the right side of the screen.

y  
In the plane of the screen, positive towards the top of the screen.

z  
Perpendicular to the screen, positive out of the screen.

This property is `null` if the device cannot provide the user acceleration—that is, if the device does not have a gyroscope.

Use the accelerationIncludingGravity property to get the total acceleration.

Note

If the device does not have a gyroscope, then you may need to implement your own gravity direction detection using a low pass filter.

## See Also

### Getting Motion Event Properties

accelerationIncludingGravity

The total acceleration of the device, which includes the user acceleration and the gravity.

interval

The interval in milliseconds since the last device motion event.

rotationRate

The rotation rate of the device.

