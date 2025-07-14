

- AVFoundation
-  AVQueuePlayer 

Class

# AVQueuePlayer

An object that plays a sequence of player items.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
@MainActor
class AVQueuePlayer
```

## Mentioned in 

Supporting AirPlay in your app

Implementing simple enhanced buffering for your content

## Overview

Use an instance of this class to manage a queue of player items.

## Topics

### Creating a Queue Player

init(items: [AVPlayerItem])

Creates an object that plays a queue of items.

### Managing the Player Queue

func items() -> [AVPlayerItem]

Returns an array of the currently enqueued items.

func advanceToNextItem()

Ends playback of the current item and starts playback of the next item in the player’s queue.

func canInsert(AVPlayerItem, after: AVPlayerItem?) -> Bool

Returns a Boolean value that indicates whether you can insert a player item into the player’s queue.

func insert(AVPlayerItem, after: AVPlayerItem?)

Inserts a player item after another player item in the queue.

func remove(AVPlayerItem)

Removes a given player item from the queue.

func removeAllItems()

Removes all player items from the queue.

## Relationships

### Inherits From

- AVPlayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Playback control

Controlling the transport behavior of a player

Play, pause, and seek through a media presentation.

class AVPlayer

An object that provides the interface to control the player’s transport behavior.

class AVPlayerItem

An object that models the timing and presentation state of an asset during playback.

class AVPlayerItemTrack

An object that represents the presentation state of an asset track during playback.

class AVPlayerLooper

An object that loops media content using a queue player.

