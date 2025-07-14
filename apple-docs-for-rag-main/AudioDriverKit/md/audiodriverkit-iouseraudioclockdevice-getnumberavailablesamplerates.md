

- AudioDriverKit
- IOUserAudioClockDevice
-  GetNumberAvailableSampleRates 

Instance Method

# GetNumberAvailableSampleRates

Gets the number of available sample rates of the clock device.

DriverKit 21.0+

``` source
size_t GetNumberAvailableSampleRates();
```

## Return Value

The number of available sample rates of the clock device.

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

GetAvailableSampleRates

Gets the available sample rates of the clock device.

