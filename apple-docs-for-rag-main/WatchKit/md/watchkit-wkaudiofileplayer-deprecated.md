

- WatchKit
-  WKAudioFilePlayer Deprecated

Class

# WKAudioFilePlayer

An object that controls playback of a single audio item.

watchOS 2.0–6.0Deprecated

``` source
class WKAudioFilePlayer
```

Deprecated

Use the AVFoundation framework’s AVPlayer and AVQueuePlayer classes instead.

## Overview

Use a player object to start and stop playback and to control the rate of playback. (The WKAudioFileQueuePlayer subclass extends the basic behavior to support playback of more than one item.)

The value of the player’s presentation-related properties are not valid until the underlying asset is loaded. Use the value of the status property to determine when it is valid to get the values of other properties. Specifically, wait until the status changes to WKAudioFilePlayerStatus.readyToPlay to access relevant properties.

The WKAudioFilePlayer class is key-value observing compliant for the currentItem, status, and rate properties. You can use an observer to detect changes to those properties and react accordingly. For information on how to observe properties using key-value observing, see Key-Value Observing Programming Guide.

## Topics

### Creating a Player

convenience init(playerItem: WKAudioFilePlayerItem)

Creates and returns a player initialized with the specified player item.

func replaceCurrentItem(with: WKAudioFilePlayerItem?)

Replaces the current player item with a different one.

### Configuring and Controlling Playback

func play()

Begins playback of the current item.

func pause()

Pauses playback of the associated item.

var rate: Float

The current rate of playback.

### Getting Information About the Player

var currentItem: WKAudioFilePlayerItem?

The player’s current item.

var status: WKAudioFilePlayerStatus

The status of the player.

var error: (any Error)?

An error that describes the cause of a failure.

### Getting Timing Information

var currentTime: TimeInterval

The elapsed time for the current playing item.

### Constants

enum WKAudioFilePlayerStatus

Constants that represent the status of the player.

## Relationships

### Inherits From

- NSObject

### Inherited By

- WKAudioFileQueuePlayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio

Playing Background Audio

Enable background audio in your app to provide a seamless playback experience.

Adding a Now Playing View

Provide a view that controls the currently playing audio from your app.

class WKInterfaceVolumeControl

An interface element that provides control of the audio volume from the watch or a paired iPhone.

PUICAutoLaunchAudioOptOut

A Boolean value that indicates whether a watchOS app should opt out of automatically launching when its companion iOS app starts playing audio content.

class WKAudioFileQueuePlayer

An object that controls playback of one or more audio items.

Deprecated

class WKAudioFilePlayerItem

An object that manages the presentation state of an audio file while it is playing.

Deprecated

class WKAudioFileAsset

An object that stores a reference to an audio file and provides metadata information about that file.

Deprecated

