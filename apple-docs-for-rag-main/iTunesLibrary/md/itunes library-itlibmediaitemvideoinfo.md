

- iTunes Library
-  ITLibMediaItemVideoInfo 

Class

# ITLibMediaItemVideoInfo

This class encapsulates the video information of a video media item.

Mac Catalyst 14.0+macOS 10.13+

``` source
class ITLibMediaItemVideoInfo
```

## Overview

Video media items include TV shows, movies, and video podcasts.

## Topics

### Getting Video Information

var videoWidth: Int

The width of the video in pixels.

var videoHeight: Int

The height of the video in pixels.

var series: String?

The name of the corresponding TV series, if the media item is an episode in a TV series.

var sortSeries: String?

The sorting name of the corresponding TV series, if the media item is an episode in a TV series.

var season: Int

The corresponding TV season, if the media item is an episode of a TV series.

var isHD: Bool

A Boolean value that indicates whether the video is high-definition.

var episode: String?

The name of the episode, if the media item is an episode of a TV series.

var episodeOrder: Int

The numerical order of the episode, if the media item is an episode of a TV series.

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

### Media Items

class ITLibMediaItem

This class describes a media item (a track) in the iTunes library, such as a song, a video, or a podcast.

class ITLibMediaEntity

This class describes a media entity, which can be a media item, such as an audio track.

class ITLibArtist

This class represents an artist, such as the performer of a song.

class ITLibArtwork

This class represents the artwork for a media item.

