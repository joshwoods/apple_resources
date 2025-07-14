

- AudioDriverKit
- IOUserAudioStream
-  GetLatency 

Instance Method

# GetLatency

DriverKit 21.0+

``` source
uint32_t GetLatency();
```

## Return Value

Returns uint32_t

## Discussion

Get the latency of the stream in sample frames.

Getting the value will be synchronized using the work queue created by the object.

