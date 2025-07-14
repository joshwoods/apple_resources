

- MusicKit
-  ApplicationMusicPlayer 

Class

# ApplicationMusicPlayer

An object your app uses to play music in a way that doesn’t affect the Music app’s state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
class ApplicationMusicPlayer
```

## Overview

The application music player plays music specifically for your app, and doesn’t affect the Music app’s state.

If your app includes a background audio mode in your `Info.plist` file, the application music player continues playing the current music item when your app moves to the background.

## Topics

### Classes

class Queue

### Instance Properties

var queue: ApplicationMusicPlayer.Queue

The playback queue for the application music player.

var transition: MusicPlayer.Transition

The transition between items for the application music player.

### Type Properties

static let shared: ApplicationMusicPlayer

The shared application music player, which plays music specifically for your app.

## Relationships

### Inherits From

- MusicPlayer

## See Also

### Playback

class SystemMusicPlayer

An object your app uses to play music by controlling the Music app’s state.

class MusicPlayer

An object your app uses to play music.

protocol PlayableMusicItem

A set of properties that a music player uses to initiate playback for a music item.

struct PlayParameters

An opaque object that represents parameters to initiate playback of a playable music item using a music player.

