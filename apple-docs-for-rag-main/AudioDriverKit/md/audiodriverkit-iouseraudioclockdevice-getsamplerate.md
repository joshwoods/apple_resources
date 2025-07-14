

- AudioDriverKit
- IOUserAudioClockDevice
-  GetSampleRate 

Instance Method

# GetSampleRate

Gets the sample rate of the clock device.

DriverKit 21.0+

``` source
double GetSampleRate();
```

## Return Value

The sample rate for the clock device.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Sample Rates

SetSampleRate

Sets the sample rate for the clock device.

SetAvailableSampleRates

Sets the available sample rates for the clock device.

GetAvailableSampleRates

Gets the available sample rates of the clock device.

GetNumberAvailableSampleRates

Gets the number of available sample rates of the clock device.

