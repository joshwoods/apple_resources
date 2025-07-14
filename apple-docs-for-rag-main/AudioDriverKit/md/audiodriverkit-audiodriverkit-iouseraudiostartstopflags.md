

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioStartStopFlags 

Enumeration

# IOUserAudioStartStopFlags

Values that indicate I/O starts or stops.

DriverKit 21.0+

``` source
enum IOUserAudioStartStopFlags : uint64_t;
```

## Topics

### Start/Stop Behaviors

None

A flag that indicates starting or stopping for normal I/O operation.

Prewarm

A flag that indicates starting or stopping for prewarming.

## See Also

### Performing I/O

StartIO

Tells the clock device to start I/O.

StopIO

Tells the clock device to stop I/O.

