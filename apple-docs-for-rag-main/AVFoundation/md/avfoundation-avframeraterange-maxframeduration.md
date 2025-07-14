

- AVFoundation
- AVFrameRateRange
-  maxFrameDuration 

Instance Property

# maxFrameDuration

The maximum frame duration supported by the range.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var maxFrameDuration: CMTime { get }
```

## Discussion

This value is the reciprocal of minFrameRate, and expresses the minimum frame rate as a duration.

## See Also

### Accessing Properties

var maxFrameRate: Float64

The maximum frame rate supported by the range.

var minFrameDuration: CMTime

The minimum frame duration supported by the range.

var minFrameRate: Float64

The minimum frame rate supported by the range.

