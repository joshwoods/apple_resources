

- CarPlay
- CPListItem
-  isPlaying 

Instance Property

# isPlaying

A Boolean value that determines whether the list item displays its Now Playing indicator.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var isPlaying: Bool { get set }
```

## Discussion

If true, the list item displays its Now Playing indicator and positions it using the location that the playingIndicatorLocation property specifies. The default value is false.

## See Also

### Managing Playback Information

var isExplicitContent: Bool

A Boolean value that determines whether the list item displays its explicit content indicator.

var playingIndicatorLocation: CPListItemPlayingIndicatorLocation

The location where the list item displays its Now Playing indicator.

enum CPListItemPlayingIndicatorLocation

The locations where a list item can display the Now Playing indicator.

var playbackProgress: CGFloat

The playback progress status for the content that the list item represents.

