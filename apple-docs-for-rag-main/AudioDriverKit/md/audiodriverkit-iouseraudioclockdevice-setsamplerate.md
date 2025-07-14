

- AudioDriverKit
- IOUserAudioClockDevice
-  SetSampleRate 

Instance Method

# SetSampleRate

Sets the sample rate for the clock device.

DriverKit 21.0+

``` source
kern_return_t SetSampleRate(double in_sample_rate);
```

## Parameters 

`in_sample_rate`  

The sample rate to set on the clock device.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the sample rate sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Sample Rates

GetSampleRate

Gets the sample rate of the clock device.

SetAvailableSampleRates

Sets the available sample rates for the clock device.

GetAvailableSampleRates

Gets the available sample rates of the clock device.

GetNumberAvailableSampleRates

Gets the number of available sample rates of the clock device.

