

- AudioDriverKit
- IOUserAudioDevice
-  GetInputSafetyOffset 

Instance Method

# GetInputSafetyOffset

Returns the input safety offset of the device.

DriverKit 21.0+

``` source
uint32_t GetInputSafetyOffset();
```

## Return Value

The input safety offset value, as a uint32_t.

## Discussion

The safety offset indicates the number for frames behind the current hardware position that’s safe to perform input I/O.

## See Also

### Working with Safety Offset Behvaior

SetInputSafetyOffset

Specifies the input safety offset of the device.

SetOutputSafetyOffset

Specifies the output safety offset of the device.

GetOutputSafetyOffset

Returns the output safety offset of the device.

