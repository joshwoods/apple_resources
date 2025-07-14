

- AudioDriverKit
- IOUserAudioLevelControl
-  HandleChangeScalarValue 

Instance Method

# HandleChangeScalarValue

Tells the slider control the scalar value is changing.

DriverKit 21.0+

``` source
kern_return_t HandleChangeScalarValue(float in_scalar_value);
```

## Parameters 

`in_scalar_value`  

The new scalar value to set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation calls SetScalarValue and returns kIOReturnSuccess. Subclass and override this method to handle changes to the stream format and return kIOReturnSuccess upon success.

## See Also

### Supporting Value Changes

HandleChangeDecibelValue

Tells the slider control the decibel value is changing.

