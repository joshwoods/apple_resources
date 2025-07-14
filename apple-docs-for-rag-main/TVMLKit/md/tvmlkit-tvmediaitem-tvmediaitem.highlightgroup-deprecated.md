

- TVMLKit
- TVMediaItem
-  TVMediaItem.HighlightGroup Deprecated

Class

# TVMediaItem.HighlightGroup

A container for groups of highlights for a media item.

tvOS 12.0–18.0Deprecated

``` source
class HighlightGroup
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Accessing the Highlights

var localizedName: String?

The name of a highlight group.

var highlights: [TVMediaItem.Highlight]

An array of the individual highlights that make up a group.

class Highlight

An object that describes a media item highlight.

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

var interstitials: [TVMediaItem.TimeRange]

An array of time intervals that indicate where to insert media items into another, single media item.

Deprecated

class TimeRange

An object that defines a time range in a media item.

Deprecated

var resumeTime: TimeInterval

The number of seconds from the beginning of a media item to the point where that media item begins playing.

Deprecated

