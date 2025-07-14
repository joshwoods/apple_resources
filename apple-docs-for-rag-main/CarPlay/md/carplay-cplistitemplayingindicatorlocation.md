

- CarPlay
-  CPListItemPlayingIndicatorLocation 

Enumeration

# CPListItemPlayingIndicatorLocation

The locations where a list item can display the Now Playing indicator.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum CPListItemPlayingIndicatorLocation
```

## Overview

Use these constants to set the value of a list item’s playingIndicatorLocation property. When you set a list item’s isPlaying property to `true`, it uses the specified location to position the Now Playing indicator.

## Topics

### Now Playing Indicator Locations

case leading

Align the Now Playing indicator with the leading edge of the list item.

case trailing

Align the Now Playing indicator with the trailing edge of the list item.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Playback Information

var isExplicitContent: Bool

A Boolean value that determines whether the list item displays its explicit content indicator.

var isPlaying: Bool

A Boolean value that determines whether the list item displays its Now Playing indicator.

var playingIndicatorLocation: CPListItemPlayingIndicatorLocation

The location where the list item displays its Now Playing indicator.

var playbackProgress: CGFloat

The playback progress status for the content that the list item represents.

