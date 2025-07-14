

- AVFoundation
-  AVMutableDateRangeMetadataGroup 

Class

# AVMutableDateRangeMetadataGroup

A mutable collection of metadata items that are valid for use within a specific range of dates.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVMutableDateRangeMetadataGroup
```

## Topics

### Configuring the Metadata

var items: [AVMetadataItem]

An array of associated metadata items.

### Configuring the Date Range

var startDate: Date

The start date for the metadata date range group.

var endDate: Date?

The end date for the metadata date range group.

## Relationships

### Inherits From

- AVDateRangeMetadataGroup

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

class AVMutableTimedMetadataGroup

A mutable collection of metadata items that are valid for use during a specific time range.

class AVDateRangeMetadataGroup

A collection of metadata items that are valid for use within a specific date range.

class AVPlayerItemMediaDataCollector

The abstract base for media data collectors.

class AVPlayerItemMetadataCollector

An object used to capture the date range metadata defined for an HTTP Live Streaming asset.

