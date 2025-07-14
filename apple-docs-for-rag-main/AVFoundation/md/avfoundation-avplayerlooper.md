

- AVFoundation
-  AVPlayerLooper 

Class

# AVPlayerLooper

An object that loops media content using a queue player.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class AVPlayerLooper
```

## Overview

You can manually implement looping playback in your app using AVQueuePlayer, but `AVPlayerLooper` provides a much simpler interface to loop a single AVPlayerItem. You create a player looper by passing it a reference to your AVQueuePlayer and a template AVPlayerItem and the looper automatically manages the looping playback of this content (see example).

```
let asset = // AVAsset with its 'duration' property value loaded
let playerItem = AVPlayerItem(asset: asset)

// Create a new player looper with the queue player and template item
playerLooper = AVPlayerLooper(player: queuePlayer, templateItem: playerItem)

// Begin looping playback
queuePlayer.play()
```

## Topics

### Creating a Player Looper

init(player: AVQueuePlayer, templateItem: AVPlayerItem, timeRange: CMTimeRange, existingItemsOrdering: AVPlayerLooper.ItemOrdering)

Creates a player looper that continuously plays the full duration of a player item while adhering to the specified ordering of existing items in the queue.

convenience init(player: AVQueuePlayer, templateItem: AVPlayerItem)

Creates a player looper that continuously plays the full duration of a player item.

convenience init(player: AVQueuePlayer, templateItem: AVPlayerItem, timeRange: CMTimeRange)

Creates a player looper that continuously plays the specified time range of a player item.

### Configuring Looping

var loopingPlayerItems: [AVPlayerItem]

An array containing replicas of the template player item used to accomplish the looping.

func disableLooping()

Disables looping for the player queue.

### Observing Looping State

var loopCount: Int

The number of times the object played the media.

var status: AVPlayerLooper.Status

A status that indicates the object’s ability to loop playback.

enum Status

Status constants that indicate whether a looper can successfully perform looping playback.

### Monitoring Errors

var error: (any Error)?

An error that describes the reason looping failed.

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

class AVQueuePlayer

An object that plays a sequence of player items.

