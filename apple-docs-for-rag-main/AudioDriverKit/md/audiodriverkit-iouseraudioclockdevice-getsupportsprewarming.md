

- AudioDriverKit
- IOUserAudioClockDevice
-  GetSupportsPrewarming 

Instance Method

# GetSupportsPrewarming

Returns a Boolean value that indicates clock device’s support for prewarming.

DriverKit 21.0+

``` source
bool GetSupportsPrewarming();
```

## Return Value

`true` if the clock device supports prewarming; `false` otherwise.

## Discussion

A device that supports prewarming can enable a minimal state that allows it to be ready to start audio I/O immediately on demand.

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Timing and Latency

SetZeroTimeStampPeriod

Sets the zero time stamp of the clock device.

GetZeroTimestampPeriod

Gets the zero time stamp of the clock device.

SetOutputLatency

Sets the output latency of the clock device.

GetOutputLatency

Gets the output latency of the clock device.

SetInputLatency

Sets the input latency of the clock device.

GetInputLatency

Get the input latency of the clock device.

