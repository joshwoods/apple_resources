

- AudioDriverKit
- IOUserAudioClockDevice
-  GetDeviceIsAlive 

Instance Method

# GetDeviceIsAlive

Gets a Boolean value that represents whether the device is alive.

DriverKit 21.0+

``` source
bool GetDeviceIsAlive();
```

## Return Value

`true` if the device is alive; `false` otherwise.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Clock Device State

GetDeviceIsRunning

Gets a Boolean value that indicates whether the device is running.

SetDeviceIsAlive

Sets a Boolean value to represent whether the device is alive.

SetIsHidden

Sets a Boolean value to indicate whether the device is hidden.

GetIsHidden

Gets a Boolean value that indicates whether the device is hidden.

