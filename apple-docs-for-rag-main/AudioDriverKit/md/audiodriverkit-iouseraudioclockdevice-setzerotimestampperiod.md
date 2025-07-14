

- AudioDriverKit
- IOUserAudioClockDevice
-  SetZeroTimeStampPeriod 

Instance Method

# SetZeroTimeStampPeriod

Sets the zero time stamp of the clock device.

DriverKit 21.0+

``` source
kern_return_t SetZeroTimeStampPeriod(uint32_t in_zts_period);
```

## Parameters 

`in_zts_period`  

The zero time stamp period.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The parameter indicates the number of sample frames the host can expect between successive timestamps returned from GetCurrentZeroTimestamp. In other words, if GetCurrentZeroTimestamp returns a sample time of `x`, the host can expect that the next valid timestamp it recieves will be `x + in_zero_timestamp_period`.

Only set this value during the PerformDeviceConfigurationChange call. If you need to change the value at any other time, call RequestDeviceConfigurationChange. This allows I/O to stop and calls PerformDeviceConfigurationChange, during which you can set the value.

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Timing and Latency

GetSupportsPrewarming

Returns a Boolean value that indicates clock device’s support for prewarming.

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

