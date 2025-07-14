

- TVMLKit
-  TVMediaItem Deprecated

Class

# TVMediaItem

A single audio or video item associated with the Apple TV JavaScript player.

tvOS 12.0–18.0Deprecated

``` source
class TVMediaItem
```

Deprecated

Please use SwiftUI or UIKit

## Overview

A `TVMediaItem` object contains read-only information about a media item associated with the JavaScript player. You can use this information with your own custom AVPlayer objects exposed through a TVPlayer object. For example, you can retrieve audio track information from the JavaScript player and play the track through a TVPlayer object.

## Topics

### Rating Media Content

var containsExplicitContent: Bool

A Boolean value indicating whether the item contains adult-oriented content.

var contentRatingDomain: TVMediaItem.ContentRatingDomain?

The media domain that the rating applies to.

struct ContentRatingDomain

A value identifying the media’s content rating domain.

var contentRatingRanking: NSNumber?

The rating for a video item.

### Identifying Media Items

var artworkImageURL: URL?

The URL path to the artwork that accompanies the media item.

var itemDescription: String?

The description for a media item.

var subtitle: String?

The subtitle for a media item.

var title: String?

The title for a media item.

var type: TVMediaItem.MediaType?

The type of media item.

struct MediaType

A value indicating whether the media is audio or video.

var url: URL?

The URL path to the media item.

var userInfo: [String : Any]

User-defined metadata, like a developer-specific identifier, for a media item.

### Setting Timing Options

var highlightGroups: [TVMediaItem.HighlightGroup]

An array containing groups of individual highlights in a media item.

class HighlightGroup

A container for groups of highlights for a media item.

var interstitials: [TVMediaItem.TimeRange]

An array of time intervals that indicate where to insert media items into another, single media item.

class TimeRange

An object that defines a time range in a media item.

var resumeTime: TimeInterval

The number of seconds from the beginning of a media item to the point where that media item begins playing.

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

### Custom Player

class TVPlaylist

A collection of media items associated with the Apple TV JavaScript player.

Deprecated

class TVPlayer

A customizable native media player used to control playback from the JavaScript player used in an Apple TV client-server app.

Deprecated

