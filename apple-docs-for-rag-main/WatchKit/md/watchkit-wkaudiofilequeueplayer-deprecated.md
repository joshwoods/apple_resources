

- WatchKit
-  WKAudioFileQueuePlayer Deprecated

Class

# WKAudioFileQueuePlayer

An object that controls playback of one or more audio items.

watchOS 2.0–6.0Deprecated

``` source
class WKAudioFileQueuePlayer
```

Deprecated

Use the AVFoundation framework’s AVPlayer and AVQueuePlayer classes instead.

## Overview

Items are stored in a queue and played sequentially. When playback of the current item ends, playback of the next item begins automatically.

Because this class is a subclass of WKAudioFilePlayer, it inherits the same playback controls and state information as its superclass. You can use the inherited methods to start and stop playback or change the playback rate. You can also get information about the current status of the player, including the elapsed playback time for the currently playing item. This method also implements the inherited replaceCurrentItem(with:) method and uses it to end playback of one item and start playback of another.

## Topics

### Creating a Queue Player

convenience init(items: [WKAudioFilePlayerItem])

Creates and returns a player initialized with an array of items.

### Managing Items

var items: [WKAudioFilePlayerItem]

The array of queued items.

func advanceToNextItem()

Ends playback of the current item and begins playing the next item in the queue.

func appendItem(WKAudioFilePlayerItem)

Adds the specified item to the end of the queue.

func removeItem(WKAudioFilePlayerItem)

Removes the specified item from the queue.

func removeAllItems()

Removes all items from the queue.

## Relationships

### Inherits From

- WKAudioFilePlayer

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

class WKAudioFilePlayerItem

An object that manages the presentation state of an audio file while it is playing.

Deprecated

class WKAudioFileAsset

An object that stores a reference to an audio file and provides metadata information about that file.

Deprecated

