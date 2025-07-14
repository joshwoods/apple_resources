

- AVFAudio
- AVAudioEngine
-  disconnectNodeOutput(\_:bus:) 

Instance Method

# disconnectNodeOutput(\_:bus:)

Removes the output connection of a node on the specified bus.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func disconnectNodeOutput(
    _ node: AVAudioNode,
    bus: AVAudioNodeBus
)
```

## Parameters 

`node`  

The audio node with the output to disconnect.

`bus`  

The destination’s output bus to disconnect.

## See Also

### Connecting and Disconnecting Audio Nodes

func connect(AVAudioNode, to: AVAudioNode, format: AVAudioFormat?)

Establishes a connection between two nodes.

func connect(AVAudioNode, to: AVAudioNode, fromBus: AVAudioNodeBus, toBus: AVAudioNodeBus, format: AVAudioFormat?)

Establishes a connection between two nodes, specifying the input and output busses.

func disconnectNodeInput(AVAudioNode)

Removes all input connections of the node.

func disconnectNodeInput(AVAudioNode, bus: AVAudioNodeBus)

Removes the input connection of a node on the specified bus.

func disconnectNodeOutput(AVAudioNode)

Removes all output connections of a node.

