

- Media Player
- MPMusicPlayerMediaItemQueueDescriptor
-  init(query:) 

Initializer

# init(query:)

Creates a new queue descriptor using the designated query.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
init(query: MPMediaQuery)
```

## Parameters 

`query`  

The query used to create the new queue descriptor.

## Return Value

A new queue descriptor consisting of the media items contained in the designated query.

## Discussion

After creating a new queue descriptor, you can modify when individual media items start and stop playing, and which item in the queue plays first when playback begins.

## See Also

### Creating a new media item queue descriptor

init(itemCollection: MPMediaItemCollection)

Creates a new queue descriptor using the designated collection.

