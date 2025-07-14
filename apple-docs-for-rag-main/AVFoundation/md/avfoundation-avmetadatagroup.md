

- AVFoundation
-  AVMetadataGroup 

Class

# AVMetadataGroup

A collection of metadata items associated with a timeline segment.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVMetadataGroup
```

## Topics

### Inspecting the Metadata Group

var items: [AVMetadataItem]

The array of metadata items associated with the metadata group.

var uniqueID: String?

The unique identifier for the metadata group.

var classifyingLabel: String?

The classifying label associated with the metadata group.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVDateRangeMetadataGroup
- AVTimedMetadataGroup

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Timed metadata

Presenting Chapter Markers

Add chapter markers to enable users to quickly navigate your content.

class AVTimedMetadataGroup

A collection of metadata items that are valid for use during a specific time range.

class AVMutableTimedMetadataGroup

A mutable collection of metadata items that are valid for use during a specific time range.

class AVDateRangeMetadataGroup

A collection of metadata items that are valid for use within a specific date range.

class AVMutableDateRangeMetadataGroup

A mutable collection of metadata items that are valid for use within a specific range of dates.

class AVPlayerItemMediaDataCollector

The abstract base for media data collectors.

class AVPlayerItemMetadataCollector

An object used to capture the date range metadata defined for an HTTP Live Streaming asset.

