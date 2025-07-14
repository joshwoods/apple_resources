

- AVFAudio
- AVAudioNode
-  removeTap(onBus:) 

Instance Method

# removeTap(onBus:)

Removes an audio tap on a bus you specify.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeTap(onBus bus: AVAudioNodeBus)
```

## Parameters 

`bus`  

The node output bus with the tap to remove.

## See Also

### Installing and Removing an Audio Tap

func installTap(onBus: AVAudioNodeBus, bufferSize: AVAudioFrameCount, format: AVAudioFormat?, block: AVAudioNodeTapBlock)

Installs an audio tap on a bus you specify to record, monitor, and observe the output of the node.

typealias AVAudioNodeTapBlock

The block that receives copies of the output of an audio node.

