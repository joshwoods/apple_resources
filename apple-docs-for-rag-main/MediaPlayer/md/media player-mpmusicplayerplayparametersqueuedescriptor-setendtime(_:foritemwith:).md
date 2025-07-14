

- Media Player
- MPMusicPlayerPlayParametersQueueDescriptor
-  setEndTime(\_:forItemWith:) 

Instance Method

# setEndTime(\_:forItemWith:)

Sets the time the item with the associated play parameters is to stop playing.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func setEndTime(
    _ endTime: TimeInterval,
    forItemWith playParameters: MPMusicPlayerPlayParameters
)
```

## Parameters 

`endTime`  

The TimeInterval describing when the item with designated play parameters stops playing.

`playParameters`  

The play parameters associated with the item in the queue that has a changed end time.

## See Also

### Setting start and end times

func setStartTime(TimeInterval, forItemWith: MPMusicPlayerPlayParameters)

Sets the time the item with the associated play parameters is to start playing.

