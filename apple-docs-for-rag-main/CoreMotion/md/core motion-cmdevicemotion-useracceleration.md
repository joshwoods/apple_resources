

- Core Motion
- CMDeviceMotion
-  userAcceleration 

Instance Property

# userAcceleration

The acceleration that the user is giving to the device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
var userAcceleration: CMAcceleration { get }
```

## Discussion

The total acceleration of the device is equal to gravity plus the acceleration the user imparts to the device.

## See Also

### Getting Acceleration Data

var gravity: CMAcceleration

The gravity acceleration vector expressed in the device’s reference frame.

