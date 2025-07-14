

- AVFoundation
- AVSampleBufferRequest
- AVSampleBufferRequest.Mode
-  AVSampleBufferRequest.Mode.opportunistic 

Case

# AVSampleBufferRequest.Mode.opportunistic

A mode that indicates that opportunistic sample buffer creation requests load data as soon as possible.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case opportunistic
```

## Discussion

In situations with multiple competing requests, a sample buffer generator may defer an opportunistic request in favor of another immediate request, or a scheduled requests with a presentation time close to the timebase time.

Important

The system may postpone an opportunistic request indefinitely. Don’t use this mode for time-sensitive processing.

## See Also

### Mode Scheduling

case immediate

A mode that indicates that sample buffer creation requests load data as soon as possible.

case scheduled

A mode that indicates that sample buffer creation requests load data according to a scheduled deadline.

