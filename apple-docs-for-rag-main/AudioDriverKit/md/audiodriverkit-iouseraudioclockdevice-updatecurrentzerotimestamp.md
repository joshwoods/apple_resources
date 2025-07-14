

- AudioDriverKit
- IOUserAudioClockDevice
-  UpdateCurrentZeroTimestamp 

Instance Method

# UpdateCurrentZeroTimestamp

Updates the current timestamp value.

DriverKit 21.0+

``` source
void UpdateCurrentZeroTimestamp(uint64_t in_sample_time, uint64_t in_host_time);
```

## Parameters 

`in_sample_time`  

The most current sample time tracked by the hardware device.

`in_host_time`  

The most current host time tracked by the hardware device.

## Discussion

Updating the current timestamp should use the time passed in the hardware interrupt.

## See Also

### Accessing Timestamps

GetCurrentZeroTimestamp

Gets the current zero timestamp value.

