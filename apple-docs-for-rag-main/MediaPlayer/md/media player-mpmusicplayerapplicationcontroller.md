

- Media Player
-  MPMusicPlayerApplicationController 

Class

# MPMusicPlayerApplicationController

A media player object that you use to revise the queue that’s currently playing.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
class MPMusicPlayerApplicationController
```

## Topics

### Changing the queue contents

func perform(queueTransaction: (MPMusicPlayerControllerMutableQueue) -> Void, completionHandler: (MPMusicPlayerControllerQueue, (any Error)?) -> Void)

Changes the contents of the media items in the queue.

static let MPMusicPlayerControllerQueueDidChange: NSNotification.Name

Indicates the music player’s queue changed.

## Relationships

### Inherits From

- MPMusicPlayerController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MPMediaPlayback
- NSObjectProtocol

## See Also

### Media player queues

class MPMusicPlayerControllerQueue

An immutable queue containing the media items to play.

class MPMusicPlayerControllerMutableQueue

A mutable queue containing the media items to play.

class MPMusicPlayerMediaItemQueueDescriptor

A set of properties and methods for modifying audio media items in the player’s media queue.

class MPMusicPlayerStoreQueueDescriptor

A set of properties and methods for modifying items, based on their store identifier, in the player’s queue.

class MPMusicPlayerPlayParametersQueueDescriptor

A set of properties and methods for modifying how to play items, based on play parameters the framework returns.

class MPMusicPlayerQueueDescriptor

The abstract base class for audio media item and store queue descriptors.

