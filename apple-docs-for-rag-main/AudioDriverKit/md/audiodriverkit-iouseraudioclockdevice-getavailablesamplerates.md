

- AudioDriverKit
- IOUserAudioClockDevice
-  GetAvailableSampleRates 

Instance Method

# GetAvailableSampleRates

Gets the available sample rates of the clock device.

DriverKit 21.0+

``` source
size_t GetAvailableSampleRates(double * out_sample_rates, size_t in_num_rates);
```

## Parameters 

`out_sample_rates`  

A pointer to a buffer of type `double` whose size corresponds to `in_num_rates`. After the call completes, this buffer contains the available sample rates.

`in_num_rates`  

The number of rates in the `out_sample_rates` buffer.

## Return Value

A `size_t` that indicates how many rates were set in the `out_sample_rates` buffer.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Sample Rates

SetSampleRate

Sets the sample rate for the clock device.

GetSampleRate

Gets the sample rate of the clock device.

SetAvailableSampleRates

Sets the available sample rates for the clock device.

GetNumberAvailableSampleRates

Gets the number of available sample rates of the clock device.

