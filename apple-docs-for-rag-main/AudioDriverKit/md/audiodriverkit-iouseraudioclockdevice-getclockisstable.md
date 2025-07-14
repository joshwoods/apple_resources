

- AudioDriverKit
- IOUserAudioClockDevice
-  GetClockIsStable 

Instance Method

# GetClockIsStable

Gets a Boolean value that represents the clock’s stability.

DriverKit 21.0+

``` source
bool GetClockIsStable();
```

## Return Value

`true` if the clock is stable; `false` otherwise.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Clock Device Behavior

SetClockAlgorithm

Sets the clock algorithm of the clock device.

GetClockAlgorithm

Gets the clock algorithm of the clock device.

IOUserAudioClockAlgorithm

Values that describe clock-smoothing algorithms.

SetClockIsStable

Sets a Boolean value to represent the clock’s stability.

