

- AVFAudio
-  AVAudioSinkNodeReceiverBlock 

Type Alias

# AVAudioSinkNodeReceiverBlock

A block that receives audio data from an audio sink node.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias AVAudioSinkNodeReceiverBlock = (UnsafePointer, AVAudioFrameCount, UnsafePointer) -> OSStatus
```

## Parameters 

`timestamp`  

The time the input data renders.

`frameCount`  

The number of sample frames of input the engine provides.

`inputData`  

The input audio data.

## Return Value

An `OSStatus` result code. When an error occurs, consider the audio data invalid.

## See Also

### Creating an Audio Sink Node

init(receiverBlock: AVAudioSinkNodeReceiverBlock)

Creates an audio sink node with a block that receives audio data.

