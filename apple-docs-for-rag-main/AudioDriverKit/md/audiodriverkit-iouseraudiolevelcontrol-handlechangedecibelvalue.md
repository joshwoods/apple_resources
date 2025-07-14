

- AudioDriverKit
- IOUserAudioLevelControl
-  HandleChangeDecibelValue 

Instance Method

# HandleChangeDecibelValue

Tells the slider control the decibel value is changing.

DriverKit 21.0+

``` source
kern_return_t HandleChangeDecibelValue(float in_decibel_value);
```

## Parameters 

`in_decibel_value`  

The new decibel value to set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation calls SetDecibelValue and returns kIOReturnSuccess. Subclass and override this method to handle changes to the stream format and return kIOReturnSuccess upon success.

## See Also

### Supporting Value Changes

HandleChangeScalarValue

Tells the slider control the scalar value is changing.

