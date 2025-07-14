

- AVFoundation
-  AVDelegatingPlaybackCoordinator 

Class

# AVDelegatingPlaybackCoordinator

A playback coordinator subclass that coordinates the playback of custom player objects in a connected group.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class AVDelegatingPlaybackCoordinator
```

## Overview

This object coordinates the state of custom player objects, such as those that render media using AVSampleBufferDisplayLayer and AVSampleBufferAudioRenderer, or that play audio using AVAudioEngine.

Adopt the AVPlaybackCoordinatorPlaybackControlDelegate protocol so that your app responds to playback commands from the coordinator. The commands provide the details of a requested state change so you can control your player object accordingly.

## Topics

### Creating a Coordinator

init(playbackControlDelegate: any AVPlaybackCoordinatorPlaybackControlDelegate)

Creates a playback coordinator for a custom playback object.

protocol AVPlaybackCoordinatorPlaybackControlDelegate

A protocol that defines the method to implement to respond to playback commands from the playback coordinator.

### Identifying Items

var currentItemIdentifier: String?

An identifier of the current item.

### Accessing the Delegate

var playbackControlDelegate: (any AVPlaybackCoordinatorPlaybackControlDelegate)?

The delegate object for the playback coordinator.

### Coordinating State Changes

func coordinateRateChange(to: Float, options: AVDelegatingPlaybackCoordinatorRateChangeOptions)

Coordinates a rate change across all participants, waiting for others to become ready, if necessary.

func coordinateSeek(to: CMTime, options: AVDelegatingPlaybackCoordinatorSeekOptions)

Coordinates a seek to the specified time for all connected participants.

func transitionToItem(withIdentifier: String?, proposingInitialTimingBasedOn: CMTimebase?)

Tells the coordinator to transition to a new item.

func reapplyCurrentItemStateToPlaybackControlDelegate()

Tells the coordinator to reissue current play state commands to synchronize the current item to the state of other participants.

struct AVDelegatingPlaybackCoordinatorSeekOptions

Constants that define seek options.

struct AVDelegatingPlaybackCoordinatorRateChangeOptions

Constants that define rate change options.

### Playback Commands

class AVDelegatingPlaybackCoordinatorPlaybackControlCommand

An abstract superclass for playback commands.

class AVDelegatingPlaybackCoordinatorPlayCommand

A command that indicates to play at a specific rate and time.

class AVDelegatingPlaybackCoordinatorPauseCommand

A command that indicates to pause playback.

class AVDelegatingPlaybackCoordinatorSeekCommand

A command that indicates to seek to a new time in the item timeline.

class AVDelegatingPlaybackCoordinatorBufferingCommand

A command that indicates to start buffering data in preparation for playback.

## Relationships

### Inherits From

- AVPlaybackCoordinator

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### SharePlay

Destination Video

Leverage SwiftUI to build an immersive media experience in a multiplatform app.

Supporting Coordinated Media Playback

Create synchronized media experiences that enable users to watch and listen across devices.

class AVPlaybackCoordinator

An object that coordinates the playback of players in a connected group.

class AVPlayerPlaybackCoordinator

A playback coordinator subclass that coordinates the playback of player objects in a connected group.

