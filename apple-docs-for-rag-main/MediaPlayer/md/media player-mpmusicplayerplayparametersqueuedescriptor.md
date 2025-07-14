

- Media Player
-  MPMusicPlayerPlayParametersQueueDescriptor 

Class

# MPMusicPlayerPlayParametersQueueDescriptor

A set of properties and methods for modifying how to play items, based on play parameters the framework returns.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
class MPMusicPlayerPlayParametersQueueDescriptor
```

## Overview

Use this class to modify the player queue created by a query before the queue begins to play. You can modify when individual items start and stop playing, along with setting the first item for playing.

## Topics

### Creating a new play parameters queue descriptor

init(playParametersQueue: [MPMusicPlayerPlayParameters])

Creates a new queue descriptor using the designated queue of play parameters.

class MPMusicPlayerPlayParameters

The MusicKit parameters that describe items to play.

### Accessing the play parameters

var playParametersQueue: [MPMusicPlayerPlayParameters]

An array containing the play parameters returned from querying MusicKit.

var startItemPlayParameters: MPMusicPlayerPlayParameters?

The item identified by the play parameters to play first.

class MPMusicPlayerPlayParameters

The MusicKit parameters that describe items to play.

### Setting start and end times

func setStartTime(TimeInterval, forItemWith: MPMusicPlayerPlayParameters)

Sets the time the item with the associated play parameters is to start playing.

func setEndTime(TimeInterval, forItemWith: MPMusicPlayerPlayParameters)

Sets the time the item with the associated play parameters is to stop playing.

## Relationships

### Inherits From

- MPMusicPlayerQueueDescriptor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Media player queues

class MPMusicPlayerControllerQueue

An immutable queue containing the media items to play.

class MPMusicPlayerControllerMutableQueue

A mutable queue containing the media items to play.

class MPMusicPlayerApplicationController

A media player object that you use to revise the queue that’s currently playing.

class MPMusicPlayerMediaItemQueueDescriptor

A set of properties and methods for modifying audio media items in the player’s media queue.

class MPMusicPlayerStoreQueueDescriptor

A set of properties and methods for modifying items, based on their store identifier, in the player’s queue.

class MPMusicPlayerQueueDescriptor

The abstract base class for audio media item and store queue descriptors.

