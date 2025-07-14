

- MusicKit
- MusicPlayer
-  MusicPlayer.State 

Class

# MusicPlayer.State

An object that exposes the observable properties of a music player.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
class State
```

## Topics

### Instance Properties

var audioVariant: AudioVariant?

The active variant that indicates the quality of audio for the current entry.

var objectWillChange: AnyPublisher&lt;Void, Never>

A publisher that emits before the object has changed.

var playbackRate: Float

The current playback rate for the player.

var playbackStatus: MusicPlayer.PlaybackStatus

The current playback status of the music player.

var repeatMode: MusicPlayer.RepeatMode?

The current repeat mode of the music player.

var shuffleMode: MusicPlayer.ShuffleMode?

The current shuffle mode of the music player.

### Type Aliases

typealias ObjectWillChangePublisher

The type of publisher that emits before the object has changed.

## Relationships

### Conforms To

- ObservableObject

