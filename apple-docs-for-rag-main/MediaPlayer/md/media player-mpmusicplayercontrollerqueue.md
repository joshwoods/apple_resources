

- Media Player
-  MPMusicPlayerControllerQueue 

Class

# MPMusicPlayerControllerQueue

An immutable queue containing the media items to play.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
class MPMusicPlayerControllerQueue
```

## Overview

An `MPMusicPlayerControllerQueue` object contains the current queue for an application queue music player. To add or remove media items from a playing queue, use perform(queueTransaction:completionHandler:). The results of the method is an `MPMusicPlayerControllerQueue` object that updates the playing queue. You don’t create your own instance of this class.

## Topics

### Inspecting queue media items

var items: [MPMediaItem]

The media items in the queue.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MPMusicPlayerControllerMutableQueue

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Media player queues

class MPMusicPlayerControllerMutableQueue

A mutable queue containing the media items to play.

class MPMusicPlayerApplicationController

A media player object that you use to revise the queue that’s currently playing.

class MPMusicPlayerMediaItemQueueDescriptor

A set of properties and methods for modifying audio media items in the player’s media queue.

class MPMusicPlayerStoreQueueDescriptor

A set of properties and methods for modifying items, based on their store identifier, in the player’s queue.

class MPMusicPlayerPlayParametersQueueDescriptor

A set of properties and methods for modifying how to play items, based on play parameters the framework returns.

class MPMusicPlayerQueueDescriptor

The abstract base class for audio media item and store queue descriptors.

