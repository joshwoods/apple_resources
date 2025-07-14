

- Media Player
-  MPMusicPlayerStoreQueueDescriptor 

Class

# MPMusicPlayerStoreQueueDescriptor

A set of properties and methods for modifying items, based on their store identifier, in the player’s queue.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
class MPMusicPlayerStoreQueueDescriptor
```

## Overview

Use this class to modify the player queue created by a query before the queue begins to play. You can modify when individual items start and stop playing, along with setting the first item to play.

## Topics

### Creating a new store queue descriptor

init(storeIDs: [String])

Creates a new queue descriptor using the designated store identifiers.

### Store identifier queue descriptor properties

var startItemID: String?

The item identified by the store identifier to play first.

var storeIDs: [String]?

An array containing the store identifiers found by the query used to create the queue descriptor.

### Setting start and end times

func setStartTime(TimeInterval, forItemWithStoreID: String)

Sets the time the designated store item is to start playing.

func setEndTime(TimeInterval, forItemWithStoreID: String)

Sets the time the designated store item is to stop playing.

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

class MPMusicPlayerPlayParametersQueueDescriptor

A set of properties and methods for modifying how to play items, based on play parameters the framework returns.

class MPMusicPlayerQueueDescriptor

The abstract base class for audio media item and store queue descriptors.

