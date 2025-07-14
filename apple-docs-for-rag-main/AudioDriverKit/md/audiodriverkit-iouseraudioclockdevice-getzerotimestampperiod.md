

- AudioDriverKit
- IOUserAudioClockDevice
-  GetZeroTimestampPeriod 

Instance Method

# GetZeroTimestampPeriod

Gets the zero time stamp of the clock device.

DriverKit 21.0+

``` source
uint32_t GetZeroTimestampPeriod();
```

## Return Value

The zero time stamp of the clock device.

## Discussion

The return value indicates the number of sample frames the host can expect between successive timestamps returned from GetCurrentZeroTimestamp. In other words, if GetCurrentZeroTimestamp returns a sample time of `x`, the host can expect that the next valid timestamp it recieves will be `x +` GetZeroTimestampPeriod.

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Timing and Latency

GetSupportsPrewarming

Returns a Boolean value that indicates clock device’s support for prewarming.

SetZeroTimeStampPeriod

Sets the zero time stamp of the clock device.

SetOutputLatency

Sets the output latency of the clock device.

GetOutputLatency

Gets the output latency of the clock device.

SetInputLatency

Sets the input latency of the clock device.

GetInputLatency

Get the input latency of the clock device.

