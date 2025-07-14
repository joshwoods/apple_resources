

- AudioDriverKit
- IOUserAudioDevice
-  GetOutputSafetyOffset 

Instance Method

# GetOutputSafetyOffset

Returns the output safety offset of the device.

DriverKit 21.0+

``` source
uint32_t GetOutputSafetyOffset();
```

## Return Value

The output safety offset value, as a uint32_t.

## Discussion

The safety offset indicates the number for frames ahead of the current hardware position that’s safe to perform output I/O.

## See Also

### Working with Safety Offset Behvaior

SetInputSafetyOffset

Specifies the input safety offset of the device.

GetInputSafetyOffset

Returns the input safety offset of the device.

SetOutputSafetyOffset

Specifies the output safety offset of the device.

