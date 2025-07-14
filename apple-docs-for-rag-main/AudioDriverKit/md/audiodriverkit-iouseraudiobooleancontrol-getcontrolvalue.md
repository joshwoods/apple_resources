

- AudioDriverKit
- IOUserAudioBooleanControl
-  GetControlValue 

Instance Method

# GetControlValue

Gets the Boolean value of the control.

DriverKit 21.0+

``` source
bool GetControlValue();
```

## Return Value

The current value of the control.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Accessing the Value

SetControlValue

Sets the Boolean value of the control.

