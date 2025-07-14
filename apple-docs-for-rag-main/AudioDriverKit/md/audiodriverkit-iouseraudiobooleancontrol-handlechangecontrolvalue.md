

- AudioDriverKit
- IOUserAudioBooleanControl
-  HandleChangeControlValue 

Instance Method

# HandleChangeControlValue

Tells the Boolean control the value is changing.

DriverKit 21.0+

``` source
kern_return_t HandleChangeControlValue(bool in_control_value);
```

## Parameters 

`in_control_value`  

The new Boolean value to set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation calls SetControlValue and returns kIOReturnSuccess. Subclass and override this method to handle changes to the stream format and return kIOReturnSuccess upon success.

