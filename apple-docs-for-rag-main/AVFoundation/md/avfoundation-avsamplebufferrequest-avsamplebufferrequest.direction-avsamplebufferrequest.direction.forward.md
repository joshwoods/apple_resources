

- AVFoundation
- AVSampleBufferRequest
- AVSampleBufferRequest.Direction
-  AVSampleBufferRequest.Direction.forward 

Case

# AVSampleBufferRequest.Direction.forward

The number of following samples may be zero or greater.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case forward
```

## Discussion

The number of following samples allowed is subject to the limitCursor, preferredMinSampleCount, and maxSampleCount property values.

## See Also

### Buffer Direction

case none

A single sample will be loaded.

case reverse

The number of previous samples may be zero or greater.

