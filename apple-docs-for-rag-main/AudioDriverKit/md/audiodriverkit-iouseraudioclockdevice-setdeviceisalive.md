

- AudioDriverKit
- IOUserAudioClockDevice
-  SetDeviceIsAlive 

Instance Method

# SetDeviceIsAlive

Sets a Boolean value to represent whether the device is alive.

DriverKit 21.0+

``` source
kern_return_t SetDeviceIsAlive(bool in_is_alive);
```

## Parameters 

`in_is_alive`  

`true` if the device is alive; otherwise, `false`.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

A `true` value means the device is ready and available. `false` means the device is unusable and will most likely go away shortly.

## See Also

### Working with Clock Device State

GetDeviceIsRunning

Gets a Boolean value that indicates whether the device is running.

GetDeviceIsAlive

Gets a Boolean value that represents whether the device is alive.

SetIsHidden

Sets a Boolean value to indicate whether the device is hidden.

GetIsHidden

Gets a Boolean value that indicates whether the device is hidden.

