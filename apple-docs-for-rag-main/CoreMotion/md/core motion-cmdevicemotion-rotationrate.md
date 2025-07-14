

- Core Motion
- CMDeviceMotion
-  rotationRate 

Instance Property

# rotationRate

The rotation rate of the device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
var rotationRate: CMRotationRate { get }
```

## Discussion

A CMRotationRate structure contains data specifying the device’s rate of rotation around three axes. The value of this property contains a measurement of gyroscope data whose bias has been removed by Core Motion algorithms. The identically name property of CMGyroData, on the other hand, gives the raw data from the gyroscope. The structure type is declared in `CMGyroData.h`.

## See Also

### Getting Attitude and Rotation Rate

var attitude: CMAttitude

The attitude of the device.

