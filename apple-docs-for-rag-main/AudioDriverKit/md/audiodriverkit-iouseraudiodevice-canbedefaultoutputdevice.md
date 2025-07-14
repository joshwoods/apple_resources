

- AudioDriverKit
- IOUserAudioDevice
-  CanBeDefaultOutputDevice 

Instance Method

# CanBeDefaultOutputDevice

Returns a Boolean value that indicates if this device can be the host’s default output device.

DriverKit 21.0+

``` source
uint32_t CanBeDefaultOutputDevice();
```

## Return Value

`true` if the host can use this device as the default output device.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Default Device Behavior

SetCanBeDefaultInputDevice

Sets a Boolean value that indicates if this device can be the host’s default input device.

CanBeDefaultInputDevice

Returns a Boolean value that indicates if this device can be the host’s default input device.

SetCanBeDefaultOutputDevice

Sets a Boolean value that indicates if this device can be the host’s default output device.

SetCanBeDefaultSystemOutputDevice

Sets a Boolean value that indicates if this device can be the system’s default output device.

CanBeDefaultSystemOutputDevice

Returns a Boolean value that indicates if this device can be the system’s default output device.

