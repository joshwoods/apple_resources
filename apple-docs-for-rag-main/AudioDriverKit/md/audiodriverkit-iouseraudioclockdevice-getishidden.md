

- AudioDriverKit
- IOUserAudioClockDevice
-  GetIsHidden 

Instance Method

# GetIsHidden

Gets a Boolean value that indicates whether the device is hidden.

DriverKit 21.0+

``` source
bool GetIsHidden();
```

## Return Value

`true` if the device is hidden; `false` otherwise.

## Discussion

This value defaults to `false` when the device initializes.

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Clock Device State

GetDeviceIsRunning

Gets a Boolean value that indicates whether the device is running.

SetDeviceIsAlive

Sets a Boolean value to represent whether the device is alive.

GetDeviceIsAlive

Gets a Boolean value that represents whether the device is alive.

SetIsHidden

Sets a Boolean value to indicate whether the device is hidden.

