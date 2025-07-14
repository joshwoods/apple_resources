

- AudioDriverKit
- IOUserAudioDevice
-  SetOutputSafetyOffset 

Instance Method

# SetOutputSafetyOffset

Specifies the output safety offset of the device.

DriverKit 21.0+

``` source
kern_return_t SetOutputSafetyOffset(uint32_t in_safety_offset);
```

## Parameters 

`in_safety_offset`  

The output safety offset value, as a uint32_t.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The safety offset indicates the number for frames ahead of the current hardware position that’s safe to perform output I/O.

## See Also

### Working with Safety Offset Behvaior

SetInputSafetyOffset

Specifies the input safety offset of the device.

GetInputSafetyOffset

Returns the input safety offset of the device.

GetOutputSafetyOffset

Returns the output safety offset of the device.

