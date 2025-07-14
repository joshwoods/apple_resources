

- AVFAudio
- AVAudioSinkNode
-  init(receiverBlock:) 

Initializer

# init(receiverBlock:)

Creates an audio sink node with a block that receives audio data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(receiverBlock block: @escaping AVAudioSinkNodeReceiverBlock)
```

## Parameters 

`block`  

The block that receives audio data from the input.

## Discussion

When connecting the audio sink node to another node, the system uses the connection format to set the audio format for the input bus.

The system calls the block on the real-time thread when receiving input data. Avoid making blocking calls within the block.

When receiving data, the system sets the audio format using the node’s input format.

## See Also

### Creating an Audio Sink Node

typealias AVAudioSinkNodeReceiverBlock

A block that receives audio data from an audio sink node.

