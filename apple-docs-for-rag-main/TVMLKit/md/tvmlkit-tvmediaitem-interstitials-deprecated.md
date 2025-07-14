

- TVMLKit
- TVMediaItem
-  interstitials Deprecated

Instance Property

# interstitials

An array of time intervals that indicate where to insert media items into another, single media item.

tvOS 12.0–18.0Deprecated

``` source
var interstitials: [TVMediaItem.TimeRange] { get }
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

The `Interstitials` property defines points within a TVMediaItem object where you can insert another media item; for example, a short ad. Each time range in the array contains two properties: startTime and duration. The `startTime` is the length of time from the beginning of a media item, in seconds. The `duration` is the length of the interstitial, in seconds. Both properties are required. A common use for these objects is to define when and where ads are to be played during a stream.

## See Also

### Setting Timing Options

var highlightGroups: [TVMediaItem.HighlightGroup]

An array containing groups of individual highlights in a media item.

Deprecated

class HighlightGroup

A container for groups of highlights for a media item.

Deprecated

class TimeRange

An object that defines a time range in a media item.

Deprecated

var resumeTime: TimeInterval

The number of seconds from the beginning of a media item to the point where that media item begins playing.

Deprecated

