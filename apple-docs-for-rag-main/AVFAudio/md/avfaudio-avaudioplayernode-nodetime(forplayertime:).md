

- AVFAudio
- AVAudioPlayerNode
-  nodeTime(forPlayerTime:) 

Instance Method

# nodeTime(forPlayerTime:)

Converts from player time to node time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func nodeTime(forPlayerTime playerTime: AVAudioTime) -> AVAudioTime?
```

## Parameters 

`playerTime`  

A time relative to the player’s start time.

## Return Value

A node time, or `nil` if the player isn’t playing.

## Discussion

For more information about this method and its inverse playerTime(forNodeTime:), see Player Timeline.

## See Also

### Converting Node and Player Times

func playerTime(forNodeTime: AVAudioTime) -> AVAudioTime?

Converts from node time to player time.

