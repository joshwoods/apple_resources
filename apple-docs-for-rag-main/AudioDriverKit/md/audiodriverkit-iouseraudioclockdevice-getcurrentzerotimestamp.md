

- AudioDriverKit
- IOUserAudioClockDevice
-  GetCurrentZeroTimestamp 

Instance Method

# GetCurrentZeroTimestamp

Gets the current zero timestamp value.

DriverKit 21.0+

``` source
void GetCurrentZeroTimestamp(uint64_t * out_sample_time, uint64_t * out_host_time);
```

## Parameters 

`out_sample_time`  

On return, the most current sample time tracked by the hardware device.

`out_host_time`  

On return, the most current host time tracked by the hardware device.

## See Also

### Accessing Timestamps

UpdateCurrentZeroTimestamp

Updates the current timestamp value.

