

- AVFoundation
-  AVCaptionGroup 

Class

# AVCaptionGroup

An object that represents zero or more captions that intersect in time.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVCaptionGroup
```

## Topics

### Creating a Caption Group

init(timeRange: CMTimeRange)

Creates a caption group with a time range.

init(captions: [AVCaption], timeRange: CMTimeRange)

Creates a caption group with captions and a time range.

### Inspecting the Caption Group

var captions: [AVCaption]

The captions associated with the caption group.

var timeRange: CMTimeRange

The time range of the caption group.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Groups

class AVCaptionGrouper

An object that analyzes the temporal overlaps of caption objects to create caption groups for each span of concurrent captions.

