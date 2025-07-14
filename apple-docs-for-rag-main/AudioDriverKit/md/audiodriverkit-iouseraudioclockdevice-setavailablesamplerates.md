

- AudioDriverKit
- IOUserAudioClockDevice
-  SetAvailableSampleRates 

Instance Method

# SetAvailableSampleRates

Sets the available sample rates for the clock device.

DriverKit 21.0+

``` source
kern_return_t SetAvailableSampleRates(const double * in_sample_rates, size_t in_num_rates);
```

## Parameters 

`in_sample_rates`  

A pointer to a buffer of `double` values containing the available sample rates.

`in_num_rates`  

The number of sample rates in `in_sample_rates` buffer.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the available sample rates sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Sample Rates

SetSampleRate

Sets the sample rate for the clock device.

GetSampleRate

Gets the sample rate of the clock device.

GetAvailableSampleRates

Gets the available sample rates of the clock device.

GetNumberAvailableSampleRates

Gets the number of available sample rates of the clock device.

