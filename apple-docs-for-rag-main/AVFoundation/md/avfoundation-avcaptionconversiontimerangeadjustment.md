

- AVFoundation
-  AVCaptionConversionTimeRangeAdjustment 

Class

# AVCaptionConversionTimeRangeAdjustment

An object that describes an adjustment to the time range of one or more captions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVCaptionConversionTimeRangeAdjustment
```

## Topics

### Accessing Time Offsets

var startTimeOffset: CMTime

The time value by which the system offsets the start times of captions to correct a problem.

var durationOffset: CMTime

The time value by which the system offsets the durations of captions to correct a problem.

## Relationships

### Inherits From

- AVCaptionConversionAdjustment

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Accessing the Adjustment Type

var adjustmentType: AVCaptionConversionAdjustment.AdjustmentType

The type of caption conversion adjustment.

struct AdjustmentType

Constants that indicate an adjustment type.

