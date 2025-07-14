

- AVFoundation
- AVCaptionConversionTimeRangeAdjustment
-  durationOffset 

Instance Property

# durationOffset

The time value by which the system offsets the durations of captions to correct a problem.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var durationOffset: CMTime { get }
```

## Discussion

The value may any numeric value, positive, negative, or zero.

## See Also

### Accessing Time Offsets

var startTimeOffset: CMTime

The time value by which the system offsets the start times of captions to correct a problem.

