

- AudioDriverKit
- IOUserAudioDevice
-  SetCanBeDefaultInputDevice 

Instance Method

# SetCanBeDefaultInputDevice

Sets a Boolean value that indicates if this device can be the host’s default input device.

DriverKit 21.0+

``` source
kern_return_t SetCanBeDefaultInputDevice(bool in_can_be_default);
```

## Parameters 

`in_can_be_default`  

`true` if the host can use this device as the default input device.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Default Device Behavior

CanBeDefaultInputDevice

Returns a Boolean value that indicates if this device can be the host’s default input device.

SetCanBeDefaultOutputDevice

Sets a Boolean value that indicates if this device can be the host’s default output device.

CanBeDefaultOutputDevice

Returns a Boolean value that indicates if this device can be the host’s default output device.

SetCanBeDefaultSystemOutputDevice

Sets a Boolean value that indicates if this device can be the system’s default output device.

CanBeDefaultSystemOutputDevice

Returns a Boolean value that indicates if this device can be the system’s default output device.

