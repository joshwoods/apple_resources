

- AudioDriverKit
- IOUserAudioBooleanControl
-  SetControlValue 

Instance Method

# SetControlValue

Sets the Boolean value of the control.

DriverKit 21.0+

``` source
kern_return_t SetControlValue(bool in_control_value);
```

## Parameters 

`in_control_value`  

The Boolean value to set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the control value sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Accessing the Value

GetControlValue

Gets the Boolean value of the control.

