

- AudioDriverKit
- IOUserAudioLevelControl
-  SetScalarValue 

Instance Method

# SetScalarValue

Sets the scalar value of the level control.

DriverKit 21.0+

``` source
kern_return_t SetScalarValue(float in_scalar);
```

## Parameters 

`in_scalar`  

The scalar value to set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the scalar value sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Accessing the Value

GetScalarValue

Gets the scalar value of the level control.

SetDecibelValue

Sets the decibel value of the level control.

GetDecibelValue

Gets the decibel value of the level control.

