

- AVFAudio
- AVAudioSourceNode
-  init(format:renderBlock:) 

Initializer

# init(format:renderBlock:)

Creates an audio source node with the audio format and a block that supplies audio data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    format: AVAudioFormat,
    renderBlock block: @escaping AVAudioSourceNodeRenderBlock
)
```

## Parameters 

`format`  

The format of the pulse-code modulated (PCM) audio data the block supplies.

`block`  

The block to supply audio data to the output.

## Discussion

When connecting the audio source node to another node, the system uses the connection format to set the audio format for the output bus.

Depending on the audio engine’s operating mode, call the block on real-time or nonreal-time threads. When rendering to a device, avoid making blocking calls within the block.

AVAudioSourceNode supports different audio formats for the block and the output, but the system only supports linear PCM conversions with sample rate, bit depth, and interleaving.

## See Also

### Creating an Audio Source Node

typealias AVAudioSourceNodeRenderBlock

A block that supplies audio data to an audio source node.

init(renderBlock: AVAudioSourceNodeRenderBlock)

Creates an audio source node with a block that supplies audio data.

