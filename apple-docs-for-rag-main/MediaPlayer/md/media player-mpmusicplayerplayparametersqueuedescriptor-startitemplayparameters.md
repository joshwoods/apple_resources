

- Media Player
- MPMusicPlayerPlayParametersQueueDescriptor
-  startItemPlayParameters 

Instance Property

# startItemPlayParameters

The item identified by the play parameters to play first.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
var startItemPlayParameters: MPMusicPlayerPlayParameters? { get set }
```

## Discussion

When this property isn’t set, the value is nil and the first item in the queue is the first item to play.

## See Also

### Accessing the play parameters

var playParametersQueue: [MPMusicPlayerPlayParameters]

An array containing the play parameters returned from querying MusicKit.

class MPMusicPlayerPlayParameters

The MusicKit parameters that describe items to play.

