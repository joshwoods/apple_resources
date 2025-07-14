

- Media Player
- MPMusicPlayerMediaItemQueueDescriptor
-  init(itemCollection:) 

Initializer

# init(itemCollection:)

Creates a new queue descriptor using the designated collection.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
init(itemCollection: MPMediaItemCollection)
```

## Parameters 

`itemCollection`  

The collection of media items used to create the new queue descriptor.

## Return Value

A new queue descriptor consisting of the media items contained in the designated collection.

## Discussion

After creating a new queue descriptor, you can modify when individual media items start and stop playing, and which item in the queue plays first when playback begins.

## See Also

### Creating a new media item queue descriptor

init(query: MPMediaQuery)

Creates a new queue descriptor using the designated query.

