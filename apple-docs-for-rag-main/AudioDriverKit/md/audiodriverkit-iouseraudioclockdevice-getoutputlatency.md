

- AudioDriverKit
- IOUserAudioClockDevice
-  GetOutputLatency 

Instance Method

# GetOutputLatency

Gets the output latency of the clock device.

DriverKit 21.0+

``` source
uint32_t GetOutputLatency();
```

## Return Value

The output latency of the clock device.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Timing and Latency

GetSupportsPrewarming

Returns a Boolean value that indicates clock device’s support for prewarming.

SetZeroTimeStampPeriod

Sets the zero time stamp of the clock device.

GetZeroTimestampPeriod

Gets the zero time stamp of the clock device.

SetOutputLatency

Sets the output latency of the clock device.

SetInputLatency

Sets the input latency of the clock device.

GetInputLatency

Get the input latency of the clock device.

