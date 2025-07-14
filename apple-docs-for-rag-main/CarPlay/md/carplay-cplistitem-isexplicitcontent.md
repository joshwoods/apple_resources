

- CarPlay
- CPListItem
-  isExplicitContent 

Instance Property

# isExplicitContent

A Boolean value that determines whether the list item displays its explicit content indicator.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var isExplicitContent: Bool { get set }
```

## Discussion

If true, the list item displays an explicit content indicator beside its primary text. The default value is false.

## See Also

### Managing Playback Information

var isPlaying: Bool

A Boolean value that determines whether the list item displays its Now Playing indicator.

var playingIndicatorLocation: CPListItemPlayingIndicatorLocation

The location where the list item displays its Now Playing indicator.

enum CPListItemPlayingIndicatorLocation

The locations where a list item can display the Now Playing indicator.

var playbackProgress: CGFloat

The playback progress status for the content that the list item represents.

