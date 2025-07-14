

- AudioDriverKit
- IOUserAudioClockDevice
-  PerformDeviceConfigurationChange 

Instance Method

# PerformDeviceConfigurationChange

Tells the clock device to handle a configuration change.

DriverKit 21.0+

``` source
kern_return_t PerformDeviceConfigurationChange(uint64_t change_action, OSObject * in_change_info);
```

## Parameters 

`change_action`  

A uint64_t that indicates the action the device object takes. This is the same value previously passed to RequestDeviceConfigurationChange. This value is purely for the clock device’s usage; the host doesn’t look at this value.

`in_change_info`  

A pointer to an OSObject about the configuration change. This is the same value previously passed to RequestDeviceConfigurationChange. This value is purely for the clock device’s usage; the host doesn’t look at this value. Retain and release this object reference as needed.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The host calls this method to allow the clock device to perform a configuration change. This call can result from a call to RequestDeviceConfigurationChange or a from change to an I/O state that requires a configuration change. Subclass and override this method to handle any custom configuration change requests, then call the superclass to update the I/O state. The framework stops I/O prior to performing the configuration change.

## See Also

### Supporting Device Configuration Changes

AbortDeviceConfigurationChange

Tells the clock device to stop handling a configuration change.

