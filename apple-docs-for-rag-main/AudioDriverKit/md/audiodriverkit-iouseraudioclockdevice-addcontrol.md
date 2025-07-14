

- AudioDriverKit
- IOUserAudioClockDevice
-  AddControl 

Instance Method

# AddControl

Adds a control to the clock device.

DriverKit 21.0+

``` source
kern_return_t AddControl(IOUserAudioControl * in_control);
```

## Parameters 

`in_control`  

The IOUserAudioControl to add to the clock device.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If adding the control succeeds, the control’s reference count increments by one.

## See Also

### Managing Audio Controls

RemoveControl

Removes a control from the clock device.

IOUserAudioControl

The base class for audio control objects.

