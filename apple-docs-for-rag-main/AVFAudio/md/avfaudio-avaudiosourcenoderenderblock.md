

- AVFAudio
-  AVAudioSourceNodeRenderBlock 

Type Alias

# AVAudioSourceNodeRenderBlock

A block that supplies audio data to an audio source node.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias AVAudioSourceNodeRenderBlock = (UnsafeMutablePointer, UnsafePointer, AVAudioFrameCount, UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`isSilence`  

The Boolean value that indicates whether the buffer contains only silence.

`timestamp`  

The HAL time the audio data renders.

`frameCount`  

The number of sample frames of audio data the engine requests.

`outputData`  

The output data.

## Return Value

An `OSStatus` result code. When returning an error, consider the audio data invalid.

## See Also

### Creating an Audio Source Node

init(renderBlock: AVAudioSourceNodeRenderBlock)

Creates an audio source node with a block that supplies audio data.

init(format: AVAudioFormat, renderBlock: AVAudioSourceNodeRenderBlock)

Creates an audio source node with the audio format and a block that supplies audio data.

