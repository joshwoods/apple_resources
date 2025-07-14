

- Media Player
- MPMusicPlayerMediaItemQueueDescriptor
-  startItem 

Instance Property

# startItem

Designates the media item to play first.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
var startItem: MPMediaItem? { get set }
```

## Discussion

When this property isn’t set, the value is nil and the first item in the queue is the first item to play.

## See Also

### Media item queue descriptor properties

var itemCollection: MPMediaItemCollection

Contains the media item collection used to create the queue descriptor.

var query: MPMediaQuery

Contains the media items found by the query used to create the queue descriptor.

