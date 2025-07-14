

- AudioDriverKit
- IOUserAudioClockDevice
-  RemoveControl 

Instance Method

# RemoveControl

Removes a control from the clock device.

DriverKit 21.0+

``` source
kern_return_t RemoveControl(IOUserAudioControl * in_control);
```

## Parameters 

`in_control`  

The IOUserAudioControl to remove from the clock device.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If removing the control succeeds, the control’s reference count decrements by one.

## See Also

### Managing Audio Controls

AddControl

Adds a control to the clock device.

IOUserAudioControl

The base class for audio control objects.

