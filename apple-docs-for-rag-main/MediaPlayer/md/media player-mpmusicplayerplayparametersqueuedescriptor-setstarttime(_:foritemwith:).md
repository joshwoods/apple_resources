

- Media Player
- MPMusicPlayerPlayParametersQueueDescriptor
-  setStartTime(\_:forItemWith:) 

Instance Method

# setStartTime(\_:forItemWith:)

Sets the time the item with the associated play parameters is to start playing.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
func setStartTime(
    _ startTime: TimeInterval,
    forItemWith playParameters: MPMusicPlayerPlayParameters
)
```

## Parameters 

`startTime`  

The TimeInterval describing when the item with designated play parameters starts playing.

`playParameters`  

The play parameters associated with the item in the queue that has a changed start time.

## See Also

### Setting start and end times

func setEndTime(TimeInterval, forItemWith: MPMusicPlayerPlayParameters)

Sets the time the item with the associated play parameters is to stop playing.

