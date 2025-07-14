

- AVFoundation
- AVSampleBufferRequest
- AVSampleBufferRequest.Direction
-  AVSampleBufferRequest.Direction.none 

Case

# AVSampleBufferRequest.Direction.none

A single sample will be loaded.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case none
```

## Discussion

When this constant is set, the limitCursor, preferredMinSampleCount, and maxSampleCount properties are ignored.

## See Also

### Buffer Direction

case forward

The number of following samples may be zero or greater.

case reverse

The number of previous samples may be zero or greater.

