

- AudioDriverKit
- IOUserAudioStream
-  SetLatency 

Instance Method

# SetLatency

DriverKit 21.0+

``` source
kern_return_t SetLatency(uint32_t in_latency);
```

## Parameters 

`in_latency`  

uint32_t latency value to set. Value is in sample frames.

## Return Value

Returns kern_return_t.

## Discussion

Set the latency of the stream in sample frames.

Drivers can change the latency of the stream dynamically. A notification will be sent to the host to update the object state if successful. Setting the value will be synchronized using the work queue created by the object.

