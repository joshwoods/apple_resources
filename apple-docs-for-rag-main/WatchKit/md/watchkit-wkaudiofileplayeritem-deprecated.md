

- WatchKit
-  WKAudioFilePlayerItem Deprecated

Class

# WKAudioFilePlayerItem

An object that manages the presentation state of an audio file while it is playing.

watchOS 2.0–6.0Deprecated

``` source
class WKAudioFilePlayerItem
```

Deprecated

Use the AVFoundation framework’s AVPlayer and AVQueuePlayer classes instead.

## Overview

Create a player item for each WKAudioFileAsset object you want to play and use the player item to observe the state of the audio during playback. You can then associate the player item with an audio queue or player object to control the playback.

The value of the player item’s presentation-related properties are not valid until the underlying asset is loaded. Use the value of the status property to determine when it is valid to get the values of other properties. Specifically, wait until the status changes to WKAudioFilePlayerItemStatus.readyToPlay to access relevant properties.

If you want to play an asset more than once within a queue of items, you must create separate player items for each placement in the queue.

## Topics

### Creating a Player Item

init(asset: WKAudioFileAsset)

Creates and returns a player item for the specified audio file asset.

### Getting Information About the Item

var asset: WKAudioFileAsset

The audio file asset being managed.

var status: WKAudioFilePlayerItemStatus

The status of the player item.

var error: (any Error)?

An error that describes the cause of a failure.

### Managing the Playback Position

var currentTime: TimeInterval

The current playback point, measured in seconds, from the beginning of the audio file.

func setCurrentTime(TimeInterval)

Sets the playback point, measured in seconds, from the beginning of the audio file.

### Accessing the Item’s Status

enum WKAudioFilePlayerItemStatus

Constants that represent the status of a player item.

## Relationships

### Inherits From

- NSObject

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

class WKAudioFilePlayer

An object that controls playback of a single audio item.

Deprecated

class WKAudioFileQueuePlayer

An object that controls playback of one or more audio items.

Deprecated

class WKAudioFileAsset

An object that stores a reference to an audio file and provides metadata information about that file.

Deprecated

