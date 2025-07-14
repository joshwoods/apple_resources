

- Media Player
- MPMusicPlayerPlayParametersQueueDescriptor
-  init(playParametersQueue:) 

Initializer

# init(playParametersQueue:)

Creates a new queue descriptor using the designated queue of play parameters.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
init(playParametersQueue: [MPMusicPlayerPlayParameters])
```

## Parameters 

`playParametersQueue`  

An array of play parameters created from the JSON information returned from a MusicKit query and used to populate the queue descriptor.

## Return Value

A new queue descriptor consisting of the items described by the play parameters.

## See Also

### Creating a new play parameters queue descriptor

class MPMusicPlayerPlayParameters

The MusicKit parameters that describe items to play.

