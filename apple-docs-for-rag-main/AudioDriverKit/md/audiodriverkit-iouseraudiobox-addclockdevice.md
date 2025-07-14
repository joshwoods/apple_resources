

- AudioDriverKit
- IOUserAudioBox
-  AddClockDevice 

Instance Method

# AddClockDevice

Adds an audio clock device to the audio box.

DriverKit 21.0+

``` source
kern_return_t AddClockDevice(IOUserAudioClockDevice * in_clock_device);
```

## Parameters 

`in_clock_device`  

The IOUserAudioClockDevice to associate with the box.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The box doesn’t own the clock device.

If adding the clock device succeeds, the clock device’s reference count increments by one.

## See Also

### Managing Box Contents

AddDevice

Adds an audio device to the audio box.

RemoveDevice

Removes an audio device from the audio box.

IOUserAudioDevice

An audio clock device object that handles the configurations for running I/O.

RemoveClockDevice

Adds an audio clock device to the audio box.

IOUserAudioClockDevice

An audio clock device object, used to synchronize and perform I/O.

