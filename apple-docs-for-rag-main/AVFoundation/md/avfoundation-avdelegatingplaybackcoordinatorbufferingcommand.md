

- AVFoundation
-  AVDelegatingPlaybackCoordinatorBufferingCommand 

Class

# AVDelegatingPlaybackCoordinatorBufferingCommand

A command that indicates to start buffering data in preparation for playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class AVDelegatingPlaybackCoordinatorBufferingCommand
```

## Overview

When your app receives this command, update its user interface to indicate that playback is buffering.

## Topics

### Accessing Command Details

var anticipatedPlaybackRate: Float

The rate at which the coordinator expects the current item to play.

var completionDueDate: Date?

The deadline by which the coordinator expects the delegate to complete execution of a command.

## Relationships

### Inherits From

- AVDelegatingPlaybackCoordinatorPlaybackControlCommand

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

class AVDelegatingPlaybackCoordinatorPlaybackControlCommand

An abstract superclass for playback commands.

class AVDelegatingPlaybackCoordinatorPlayCommand

A command that indicates to play at a specific rate and time.

class AVDelegatingPlaybackCoordinatorPauseCommand

A command that indicates to pause playback.

class AVDelegatingPlaybackCoordinatorSeekCommand

A command that indicates to seek to a new time in the item timeline.

