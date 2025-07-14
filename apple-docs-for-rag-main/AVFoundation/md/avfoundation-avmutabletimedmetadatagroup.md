

- AVFoundation
-  AVMutableTimedMetadataGroup 

Class

# AVMutableTimedMetadataGroup

A mutable collection of metadata items that are valid for use during a specific time range.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVMutableTimedMetadataGroup
```

## Topics

### Configuring the Group

var items: [AVMetadataItem]

An array of metadata items in the timed metadata group.

var timeRange: CMTimeRange

The time range of the timed metadata.

## Relationships

### Inherits From

- AVTimedMetadataGroup

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Timed metadata

Presenting Chapter Markers

Add chapter markers to enable users to quickly navigate your content.

class AVMetadataGroup

A collection of metadata items associated with a timeline segment.

class AVTimedMetadataGroup

A collection of metadata items that are valid for use during a specific time range.

class AVDateRangeMetadataGroup

A collection of metadata items that are valid for use within a specific date range.

class AVMutableDateRangeMetadataGroup

A mutable collection of metadata items that are valid for use within a specific range of dates.

class AVPlayerItemMediaDataCollector

The abstract base for media data collectors.

class AVPlayerItemMetadataCollector

An object used to capture the date range metadata defined for an HTTP Live Streaming asset.

