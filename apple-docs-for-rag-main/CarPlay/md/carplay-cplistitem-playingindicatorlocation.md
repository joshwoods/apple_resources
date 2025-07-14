

- CarPlay
- CPListItem
-  playingIndicatorLocation 

Instance Property

# playingIndicatorLocation

The location where the list item displays its Now Playing indicator.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var playingIndicatorLocation: CPListItemPlayingIndicatorLocation { get set }
```

## Discussion

If the list item’s isPlaying property is set to true, it uses the value of this property to position its Now Playing indicator. The default value is CPListItemPlayingIndicatorLocation.leading.

## See Also

### Managing Playback Information

var isExplicitContent: Bool

A Boolean value that determines whether the list item displays its explicit content indicator.

var isPlaying: Bool

A Boolean value that determines whether the list item displays its Now Playing indicator.

enum CPListItemPlayingIndicatorLocation

The locations where a list item can display the Now Playing indicator.

var playbackProgress: CGFloat

The playback progress status for the content that the list item represents.

