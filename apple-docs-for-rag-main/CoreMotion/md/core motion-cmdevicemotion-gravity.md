

- Core Motion
- CMDeviceMotion
-  gravity 

Instance Property

# gravity

The gravity acceleration vector expressed in the device’s reference frame.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
var gravity: CMAcceleration { get }
```

## Discussion

The total acceleration of the device is equal to gravity plus the acceleration the user imparts to the device (userAcceleration).

## See Also

### Getting Acceleration Data

var userAcceleration: CMAcceleration

The acceleration that the user is giving to the device.

