

- AudioDriverKit
- IOUserAudioClockDevice
-  SetInputLatency 

Instance Method

# SetInputLatency

Sets the input latency of the clock device.

DriverKit 21.0+

``` source
kern_return_t SetInputLatency(uint32_t in_latency);
```

## Parameters 

`in_latency`  

The input latency value to set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

Drivers can change the input latency of the clock device dynamically. If successful, changing the available input latency sends a notification to the host to update the object state.

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

GetOutputLatency

Gets the output latency of the clock device.

GetInputLatency

Get the input latency of the clock device.

