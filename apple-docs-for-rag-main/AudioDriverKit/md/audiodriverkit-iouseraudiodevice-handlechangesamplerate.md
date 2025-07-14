

- AudioDriverKit
- IOUserAudioDevice
-  HandleChangeSampleRate 

Instance Method

# HandleChangeSampleRate

Tells the device the sample rate is changing.

DriverKit 21.0+

``` source
kern_return_t HandleChangeSampleRate(double in_sample_rate);
```

## Parameters 

`in_sample_rate`  

The sample rate to set, if possible, as a `double`.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation calls SetSampleRate and returns kIOReturnSuccess. Subclass and override this method to handle changes to the sample rate and return kIOReturnSuccess upon success.

## See Also

### Supporting Sample Rate Changes

DeviceSampleRateChanged

Updates stream formats, in response to the owning audio device changing its sample rate.

