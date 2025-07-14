

- AudioDriverKit
- IOUserAudioBox
-  RemoveDevice 

Instance Method

# RemoveDevice

Removes an audio device from the audio box.

DriverKit 21.0+

``` source
kern_return_t RemoveDevice(IOUserAudioDevice * in_device);
```

## Parameters 

`in_device`  

The IOUserAudioDevice to disassociate from the box.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If removing the device succeeds, the device’s reference count decrements by one.

## See Also

### Managing Box Contents

AddDevice

Adds an audio device to the audio box.

IOUserAudioDevice

An audio clock device object that handles the configurations for running I/O.

AddClockDevice

Adds an audio clock device to the audio box.

RemoveClockDevice

Adds an audio clock device to the audio box.

IOUserAudioClockDevice

An audio clock device object, used to synchronize and perform I/O.

