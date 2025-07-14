

- AudioDriverKit
- IOUserAudioStream
-  DeviceSampleRateChanged 

Instance Method

# DeviceSampleRateChanged

Updates stream formats, in response to the owning audio device changing its sample rate.

DriverKit 21.0+

``` source
kern_return_t DeviceSampleRateChanged(double in_sample_rate);
```

## Parameters 

`in_sample_rate`  

The new sample rate.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

This method goes through all the available stream formats and selects the closet format with the matching sample rate.

Calling this method results in a call to the stream’s HandleChangeCurrentStreamFormat to update its format.

## See Also

### Supporting Sample Rate Changes

HandleChangeSampleRate

Tells the device the sample rate is changing.

