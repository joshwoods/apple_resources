

- AudioDriverKit
- IOUserAudioClockDevice
-  GetClockAlgorithm 

Instance Method

# GetClockAlgorithm

Gets the clock algorithm of the clock device.

DriverKit 21.0+

``` source
IOUserAudioClockAlgorithm GetClockAlgorithm();
```

## Return Value

The clock algorithm of the clock device.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Clock Device Behavior

SetClockAlgorithm

Sets the clock algorithm of the clock device.

IOUserAudioClockAlgorithm

Values that describe clock-smoothing algorithms.

SetClockIsStable

Sets a Boolean value to represent the clock’s stability.

GetClockIsStable

Gets a Boolean value that represents the clock’s stability.

