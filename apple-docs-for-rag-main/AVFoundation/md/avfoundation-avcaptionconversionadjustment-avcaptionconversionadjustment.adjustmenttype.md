

- AVFoundation
- AVCaptionConversionAdjustment
-  AVCaptionConversionAdjustment.AdjustmentType 

Structure

# AVCaptionConversionAdjustment.AdjustmentType

Constants that indicate an adjustment type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct AdjustmentType
```

## Topics

### Adjustment Types

static let timeRange: AVCaptionConversionAdjustment.AdjustmentType

Indicates a timing adjustment.

### Initializers

init(rawValue: String)

Creates an adjustment type with a string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing the Adjustment Type

var adjustmentType: AVCaptionConversionAdjustment.AdjustmentType

The type of caption conversion adjustment.

class AVCaptionConversionTimeRangeAdjustment

An object that describes an adjustment to the time range of one or more captions.

