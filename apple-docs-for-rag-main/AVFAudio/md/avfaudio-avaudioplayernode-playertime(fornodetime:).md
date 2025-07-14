

- AVFAudio
- AVAudioPlayerNode
-  playerTime(forNodeTime:) 

Instance Method

# playerTime(forNodeTime:)

Converts from node time to player time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func playerTime(forNodeTime nodeTime: AVAudioTime) -> AVAudioTime?
```

## Parameters 

`nodeTime`  

The node time.

## Return Value

A time relative to the player’s start time, or `nil` if the player isn’t playing.

## Discussion

For more information about this method and its inverse nodeTime(forPlayerTime:), see Player Timeline.

## See Also

### Converting Node and Player Times

func nodeTime(forPlayerTime: AVAudioTime) -> AVAudioTime?

Converts from player time to node time.

