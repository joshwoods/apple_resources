

- AudioDriverKit
- IOUserAudioDriver
-  StartDevice 

Instance Method

# StartDevice

Tells the driver to start I/O on an audio device or audio clock device.

DriverKit 21.0+

``` source
kern_return_t StartDevice(IOUserAudioObjectID in_object_id, IOUserAudioStartStopFlags in_flags);
```

## Parameters 

`in_object_id`  

The identifier of the device on which to start I/O.

`in_flags`  

A flag that indicates how to perform the I/O start operation.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation always returns kIOReturnSuccess. Subclass and override this method to handle hardware-specific startup, then call the superclass to update the I/O state. The framework expects this call to always succeed for fail. The hardware can take as long as it needs in this call, provided it always either succeeds or fails.

This call results in a call to StartIO on the device.

## See Also

### Starting and Stopping the Driver

StopDevice

Tells the driver to stop I/O on an audio device or audio clock device.

IOUserAudioObjectID

An identifier that provides a handle on a specific audio object.

IOUserAudioStartStopFlags

Values that indicate I/O starts or stops.

