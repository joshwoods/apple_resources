

- AudioDriverKit
- IOUserAudioClockDevice
-  SetClockAlgorithm 

Instance Method

# SetClockAlgorithm

Sets the clock algorithm of the clock device.

DriverKit 21.0+

``` source
kern_return_t SetClockAlgorithm(IOUserAudioClockAlgorithm in_clock_algorithm);
```

## Parameters 

`in_clock_algorithm`  

The clock algorithm to set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

Drivers can change the transport type of the clock device dynamically. If successful, changing the transport type sends a notification to the host to update the object state.

## See Also

### Working with Clock Device Behavior

GetClockAlgorithm

Gets the clock algorithm of the clock device.

IOUserAudioClockAlgorithm

Values that describe clock-smoothing algorithms.

SetClockIsStable

Sets a Boolean value to represent the clock’s stability.

GetClockIsStable

Gets a Boolean value that represents the clock’s stability.

