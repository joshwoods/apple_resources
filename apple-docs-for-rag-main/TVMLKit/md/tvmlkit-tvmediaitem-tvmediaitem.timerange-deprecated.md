

- TVMLKit
- TVMediaItem
-  TVMediaItem.TimeRange Deprecated

Class

# TVMediaItem.TimeRange

An object that defines a time range in a media item.

tvOS 12.0–18.0Deprecated

``` source
class TimeRange
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Defining the Time Range

var startTime: TimeInterval

The time in a media item that determines when a time range begins.

var endTime: TimeInterval

The time in a media item that determines when a time range ends.

var duration: TimeInterval

The duration of a time range in a media item.

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

### Setting Timing Options

var highlightGroups: [TVMediaItem.HighlightGroup]

An array containing groups of individual highlights in a media item.

Deprecated

class HighlightGroup

A container for groups of highlights for a media item.

Deprecated

var interstitials: [TVMediaItem.TimeRange]

An array of time intervals that indicate where to insert media items into another, single media item.

Deprecated

var resumeTime: TimeInterval

The number of seconds from the beginning of a media item to the point where that media item begins playing.

Deprecated

