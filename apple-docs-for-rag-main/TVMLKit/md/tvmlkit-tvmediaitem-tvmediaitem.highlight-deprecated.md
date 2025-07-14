

- TVMLKit
- TVMediaItem
-  TVMediaItem.Highlight Deprecated

Class

# TVMediaItem.Highlight

An object that describes a media item highlight.

tvOS 12.0–18.0Deprecated

``` source
class Highlight
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Accessing a Highlight

var highlightDescription: String?

A description for an individual highlight.

var imageURL: URL?

The URL for an image associated with a highlight.

var localizedName: String?

The name associated with a highlight.

var timeRange: TVMediaItem.TimeRange

A time range that determines when a highlight begins and its duration.

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

### Accessing the Highlights

var localizedName: String?

The name of a highlight group.

Deprecated

var highlights: [TVMediaItem.Highlight]

An array of the individual highlights that make up a group.

Deprecated

