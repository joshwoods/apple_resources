

- Media Player
-  MPSkipIntervalCommand 

Class

# MPSkipIntervalCommand

An object that defines the skip intervals for the player.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
class MPSkipIntervalCommand
```

## Overview

You use a skip interval to move the playback of a media item, forward or backward, the indicated number of seconds. For example, a forward skip interval of 30 seconds at 2 minutes and 30 seconds into a song would immediately jump to 3 minutes into the song and continue playing. The skipped content isn’t played.

## Topics

### Retrieving skip intervals

var preferredIntervals: [NSNumber]

The available skip intervals, in seconds, for a media item.

## Relationships

### Inherits From

- MPRemoteCommand

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Responding to track navigation events

class MPChangePlaybackPositionCommand

An object that responds to requests to change the current playback position of the playing item.

class MPChangePlaybackPositionCommandEvent

An event requesting a change in the playback position.

class MPSeekCommandEvent

An event requesting that the player seek to a new position.

class MPSkipIntervalCommandEvent

An event requesting a change in the current skip interval.

