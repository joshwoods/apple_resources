

- Media Player
-  MPMediaPlayback 

Protocol

# MPMediaPlayback

A protocol that defines the interface for controlling audio media playback.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
protocol MPMediaPlayback
```

## Mentioned in 

Playing audio using the built-in music player

## Overview

This protocol supports basic transport operations including start, stop, and pause, and also lets you seek forward and back through media or to a specific point in its timeline.

## Topics

### Starting and stopping playback

func play()

Initiates playback of the current item.

**Required**

func pause()

Pauses playback of the current item.

**Required**

func stop()

Ends playback of the current item.

**Required**

func prepareToPlay()

Prepares a media player for playback.

**Required**

var isPreparedToPlay: Bool

A Boolean value indicating whether a media player is ready to play.

**Required**

### Seeking within media

func beginSeekingBackward()

Begins seeking backward through the media content.

**Required**

func beginSeekingForward()

Begins seeking forward through the media content.

**Required**

func endSeeking()

Ends forward and backward seeking through the media content.

**Required**

### Accessing playback attributes

var currentPlaybackRate: Float

The current playback rate for the player.

**Required**

var currentPlaybackTime: TimeInterval

The current position of the playhead.

**Required**

## Relationships

### Conforming Types

- MPMoviePlayerController
- MPMusicPlayerApplicationController
- MPMusicPlayerController

## See Also

### Built-in music playback

Playing audio using the built-in music player

Create a media player inside your app to play audio from the user’s media library.

class MPMusicPlayerController

An object that plays audio media items from the device’s Music app library.

protocol MPSystemMusicPlayerController

A protocol for playing videos in the Music app.

