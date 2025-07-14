

- Media Player
-  MPMusicPlayerQueueDescriptor 

Class

# MPMusicPlayerQueueDescriptor

The abstract base class for audio media item and store queue descriptors.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
class MPMusicPlayerQueueDescriptor
```

## Relationships

### Inherits From

- NSObject

### Inherited By

- MPMusicPlayerMediaItemQueueDescriptor
- MPMusicPlayerPlayParametersQueueDescriptor
- MPMusicPlayerStoreQueueDescriptor

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

class MPMusicPlayerPlayParametersQueueDescriptor

A set of properties and methods for modifying how to play items, based on play parameters the framework returns.

