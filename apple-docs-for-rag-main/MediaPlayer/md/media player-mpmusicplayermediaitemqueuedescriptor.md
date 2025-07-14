

- Media Player
-  MPMusicPlayerMediaItemQueueDescriptor 

Class

# MPMusicPlayerMediaItemQueueDescriptor

A set of properties and methods for modifying audio media items in the player’s media queue.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MPMusicPlayerMediaItemQueueDescriptor
```

## Overview

Use this class to modify the player queue created by a query before the queue begins to play. You can modify when individual items start and stop playing, along with setting the first item to play.

## Topics

### Creating a new media item queue descriptor

init(itemCollection: MPMediaItemCollection)

Creates a new queue descriptor using the designated collection.

init(query: MPMediaQuery)

Creates a new queue descriptor using the designated query.

### Media item queue descriptor properties

var itemCollection: MPMediaItemCollection

Contains the media item collection used to create the queue descriptor.

var query: MPMediaQuery

Contains the media items found by the query used to create the queue descriptor.

var startItem: MPMediaItem?

Designates the media item to play first.

### Setting start and end times

func setStartTime(TimeInterval, for: MPMediaItem)

The time the designated media item is to start playing.

func setEndTime(TimeInterval, for: MPMediaItem)

The time the designated media item is to stop playing.

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

class MPMusicPlayerStoreQueueDescriptor

A set of properties and methods for modifying items, based on their store identifier, in the player’s queue.

class MPMusicPlayerPlayParametersQueueDescriptor

A set of properties and methods for modifying how to play items, based on play parameters the framework returns.

class MPMusicPlayerQueueDescriptor

The abstract base class for audio media item and store queue descriptors.

