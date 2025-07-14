

- Media Player
- MPMusicPlayerStoreQueueDescriptor
-  setStartTime(\_:forItemWithStoreID:) 

Instance Method

# setStartTime(\_:forItemWithStoreID:)

Sets the time the designated store item is to start playing.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func setStartTime(
    _ startTime: TimeInterval,
    forItemWithStoreID storeID: String
)
```

## Parameters 

`startTime`  

The TimeInterval describing when the store item starts playing.

`storeID`  

The store identifier associated with the item in the queue that has a changed start time.

## See Also

### Setting start and end times

func setEndTime(TimeInterval, forItemWithStoreID: String)

Sets the time the designated store item is to stop playing.

