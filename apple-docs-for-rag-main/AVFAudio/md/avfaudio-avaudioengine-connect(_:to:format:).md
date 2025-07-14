

- AVFAudio
- AVAudioEngine
-  connect(\_:to:format:) 

Instance Method

# connect(\_:to:format:)

Establishes a connection between two nodes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func connect(
    _ node1: AVAudioNode,
    to node2: AVAudioNode,
    format: AVAudioFormat?
)
```

## Parameters 

`node1`  

The source audio node.

`node2`  

The destination audio node.

`format`  

If not `NULL`, the engine uses this value for the format of the source audio node’s output bus. In all cases, the engine matches the format of the destination audio node’s input bus to the source audio node’s output bus.

## Discussion

This method calls connect(_:to:fromBus:toBus:format:) using bus `0` for the source audio node, and bus `0` for the destination audio node, except when a destination is a mixer, in which case, the destination is the mixer’s nextAvailableInputBus.

## See Also

### Connecting and Disconnecting Audio Nodes

func connect(AVAudioNode, to: AVAudioNode, fromBus: AVAudioNodeBus, toBus: AVAudioNodeBus, format: AVAudioFormat?)

Establishes a connection between two nodes, specifying the input and output busses.

func disconnectNodeInput(AVAudioNode)

Removes all input connections of the node.

func disconnectNodeInput(AVAudioNode, bus: AVAudioNodeBus)

Removes the input connection of a node on the specified bus.

func disconnectNodeOutput(AVAudioNode)

Removes all output connections of a node.

func disconnectNodeOutput(AVAudioNode, bus: AVAudioNodeBus)

Removes the output connection of a node on the specified bus.

