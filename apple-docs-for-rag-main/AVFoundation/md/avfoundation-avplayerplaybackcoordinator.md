

- AVFoundation
-  AVPlayerPlaybackCoordinator 

Class

# AVPlayerPlaybackCoordinator

A playback coordinator subclass that coordinates the playback of player objects in a connected group.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class AVPlayerPlaybackCoordinator
```

## Overview

This object coordinates the state of AVPlayer objects. You don’t create an instance of the coordinator, but instead access the player’s instance through its playbackCoordinator property.

Use the standard interfaces of AVPlayer to control playback in your app. The coordinator automatically intercepts calls that affect transport control state, like setRate(_:time:atHostTime:), pause(), and seek(to:completionHandler:), and propagates them to other participants in the group when appropriate. Similarly, the coordinator observes rate and time changes from other participants and imposes them on the player. If this occurs, the player item posts notifications that identify the originating participant.

This object may automatically suspend coordinated playback when a system state change causes the player’s timeControlStatus value to change from a playing state to a waiting or paused state. A suspension that begins because the player enters a waiting state due to an event like a network stall or interstitial playback, ends automatically when the player finishes waiting. However, if the system pauses playback due to a system state change, such as an audio session interruption, the suspension ends only after the player’s rate changes back to nonzero.

Important

A playback coordinator doesn’t manage the playback queue of connected players. You need to implement custom logic to enqueue the same item across all connected players.

## Topics

### Accessing the Player

var player: AVPlayer?

A player that participates in coordinated playback.

### Configuring the Delegate

var delegate: (any AVPlayerPlaybackCoordinatorDelegate)?

A delegate object for the playback coordinator.

protocol AVPlayerPlaybackCoordinatorDelegate

A protocol that defines the methods to implement to participate in playback coordination.

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

class AVDelegatingPlaybackCoordinator

A playback coordinator subclass that coordinates the playback of custom player objects in a connected group.

