

- AudioDriverKit
- IOUserAudioClockDevice
-  SetClockIsStable 

Instance Method

# SetClockIsStable

Sets a Boolean value to represent the clock’s stability.

DriverKit 21.0+

``` source
kern_return_t SetClockIsStable(bool in_clock_is_stable);
```

## Parameters 

`in_clock_is_stable`  

`true` if the clock is stable; otherwise, `false`.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

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

GetClockIsStable

Gets a Boolean value that represents the clock’s stability.

