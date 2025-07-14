

- AVFoundation
- AVSampleBufferRequest
- AVSampleBufferRequest.Direction
-  AVSampleBufferRequest.Direction.reverse 

Case

# AVSampleBufferRequest.Direction.reverse

The number of previous samples may be zero or greater.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case reverse
```

## Discussion

The number of previous samples allowed is subject to the limitCursor, preferredMinSampleCount, and maxSampleCount property values.

## See Also

### Buffer Direction

case forward

The number of following samples may be zero or greater.

case none

A single sample will be loaded.

