

- AudioDriverKit
- IOUserAudioClockDevice
-  SetIsHidden 

Instance Method

# SetIsHidden

Sets a Boolean value to indicate whether the device is hidden.

DriverKit 21.0+

``` source
kern_return_t SetIsHidden(bool in_is_hidden);
```

## Parameters 

`in_is_hidden`  

`true` if the device is hidden; otherwise, `false`.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

A true value indicates the device isn’t included in the normal list of devices, and is only findable by its UID. A hidden device can’t be the default device.

## See Also

### Working with Clock Device State

GetDeviceIsRunning

Gets a Boolean value that indicates whether the device is running.

SetDeviceIsAlive

Sets a Boolean value to represent whether the device is alive.

GetDeviceIsAlive

Gets a Boolean value that represents whether the device is alive.

GetIsHidden

Gets a Boolean value that indicates whether the device is hidden.

