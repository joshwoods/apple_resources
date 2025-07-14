

- iTunes Library
- ITLibMediaItemVideoInfo
-  sortSeries 

Instance Property

# sortSeries

The sorting name of the corresponding TV series, if the media item is an episode in a TV series.

Mac Catalyst 14.0+macOS 10.13+

``` source
var sortSeries: String? { get }
```

## Discussion

This property is `nil` if the media item isn’t an episode in a TV series, or if the TV series doesn’t have a sorting name.

## See Also

### Getting Video Information

var videoWidth: Int

The width of the video in pixels.

var videoHeight: Int

The height of the video in pixels.

var series: String?

The name of the corresponding TV series, if the media item is an episode in a TV series.

var season: Int

The corresponding TV season, if the media item is an episode of a TV series.

var isHD: Bool

A Boolean value that indicates whether the video is high-definition.

var episode: String?

The name of the episode, if the media item is an episode of a TV series.

var episodeOrder: Int

The numerical order of the episode, if the media item is an episode of a TV series.

