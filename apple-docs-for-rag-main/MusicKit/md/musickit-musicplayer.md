

- MusicKit
-  MusicPlayer 

Class

# MusicPlayer

An object your app uses to play music.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
class MusicPlayer
```

## Topics

### Classes

class Queue

A representation of the playback queue for a music player.

class State

An object that exposes the observable properties of a music player.

### Instance Properties

var isPreparedToPlay: Bool

A Boolean value that indicates whether a music player is ready to play.

var playbackTime: TimeInterval

The current playback time, in seconds, of the current entry.

let state: MusicPlayer.State

An object that exposes the observable properties of the music player.

### Instance Methods

func beginSeekingBackward()

Begins seeking backward through the music content.

func beginSeekingForward()

Begins seeking forward through the music content.

func endSeeking()

Ends forward and backward seeking through the music content.

func pause()

Pauses playback of the current entry.

func play() async throws

Initiates playback from the current queue.

func prepareToPlay() async throws

Prepares the current queue for playback, interrupting any active (nonmixable) audio sessions.

func restartCurrentEntry()

Restarts playback at the beginning of the currently playing entry.

func skipToNextEntry() async throws

Starts playback of the next entry in the playback queue.

func skipToPreviousEntry() async throws

Starts playback of the previous entry in the playback queue.

func stop()

Ends playback of the current entry.

### Enumerations

enum PlaybackStatus

The music player playback status modes.

enum RepeatMode

The repeat modes for the music player.

enum ShuffleMode

The shuffle modes for the music player.

enum Transition

The transition applied between playing items.

## Relationships

### Inherited By

- ApplicationMusicPlayer
- SystemMusicPlayer

## See Also

### Playback

class ApplicationMusicPlayer

An object your app uses to play music in a way that doesn’t affect the Music app’s state.

class SystemMusicPlayer

An object your app uses to play music by controlling the Music app’s state.

protocol PlayableMusicItem

A set of properties that a music player uses to initiate playback for a music item.

struct PlayParameters

An opaque object that represents parameters to initiate playback of a playable music item using a music player.

