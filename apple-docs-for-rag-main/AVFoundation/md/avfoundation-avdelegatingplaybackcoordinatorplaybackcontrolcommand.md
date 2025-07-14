

- AVFoundation
-  AVDelegatingPlaybackCoordinatorPlaybackControlCommand 

Class

# AVDelegatingPlaybackCoordinatorPlaybackControlCommand

An abstract superclass for playback commands.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class AVDelegatingPlaybackCoordinatorPlaybackControlCommand
```

## Overview

Playback commands inherit state that identifies their originator and applicable item.

## Topics

### Accessing Command Details

var expectedCurrentItemIdentifier: String

An item identifier the coordinator issues the command for.

var originator: AVCoordinatedPlaybackParticipant?

The participant that causes the coordinator to issue the command.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVDelegatingPlaybackCoordinatorBufferingCommand
- AVDelegatingPlaybackCoordinatorPauseCommand
- AVDelegatingPlaybackCoordinatorPlayCommand
- AVDelegatingPlaybackCoordinatorSeekCommand

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Playback Commands

class AVDelegatingPlaybackCoordinatorPlayCommand

A command that indicates to play at a specific rate and time.

class AVDelegatingPlaybackCoordinatorPauseCommand

A command that indicates to pause playback.

class AVDelegatingPlaybackCoordinatorSeekCommand

A command that indicates to seek to a new time in the item timeline.

class AVDelegatingPlaybackCoordinatorBufferingCommand

A command that indicates to start buffering data in preparation for playback.

