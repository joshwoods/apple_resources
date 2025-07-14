

- TVMLKit
- TVMediaItem
-  highlightGroups Deprecated

Instance Property

# highlightGroups

An array containing groups of individual highlights in a media item.

tvOS 12.0–18.0Deprecated

``` source
var highlightGroups: [TVMediaItem.HighlightGroup] { get }
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

The `highlightGroups` property enables you to show several groups highlights from a stream. Each highlight group in the array contains a list of highlights. Each highlight is an object with the following properties: highlightDescription, localizedName, imageURL, and TVMediaItem.TimeRange.

For example, consider a video of a baseball game, which is the media item. You can create a highlight group containing the video for each home run —each highlight— in the game. You create another highlight group containing all of the errors. You put these highlight groups into the highlightGroups property.

## See Also

### Setting Timing Options

class HighlightGroup

A container for groups of highlights for a media item.

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

