

- Media Player
- MPMusicPlayerStoreQueueDescriptor
-  setEndTime(\_:forItemWithStoreID:) 

Instance Method

# setEndTime(\_:forItemWithStoreID:)

Sets the time the designated store item is to stop playing.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func setEndTime(
    _ endTime: TimeInterval,
    forItemWithStoreID storeID: String
)
```

## Parameters 

`endTime`  

The TimeInterval describing when the store item stops playing.

`storeID`  

The store identifier associated with the item in the queue that has a changed end time.

## See Also

### Setting start and end times

func setStartTime(TimeInterval, forItemWithStoreID: String)

Sets the time the designated store item is to start playing.

