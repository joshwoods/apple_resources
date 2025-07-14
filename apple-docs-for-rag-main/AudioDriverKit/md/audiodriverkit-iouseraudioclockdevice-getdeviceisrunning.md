

- AudioDriverKit
- IOUserAudioClockDevice
-  GetDeviceIsRunning 

Instance Method

# GetDeviceIsRunning

Gets a Boolean value that indicates whether the device is running.

DriverKit 21.0+

``` source
bool GetDeviceIsRunning();
```

## Return Value

`true` if the device is running; `false` otherwise.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Clock Device State

SetDeviceIsAlive

Sets a Boolean value to represent whether the device is alive.

GetDeviceIsAlive

Gets a Boolean value that represents whether the device is alive.

SetIsHidden

Sets a Boolean value to indicate whether the device is hidden.

GetIsHidden

Gets a Boolean value that indicates whether the device is hidden.

