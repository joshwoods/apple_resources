

- AVFAudio
- AVAudioEngine
-  disconnectNodeInput(\_:) 

Instance Method

# disconnectNodeInput(\_:)

Removes all input connections of the node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func disconnectNodeInput(_ node: AVAudioNode)
```

## Parameters 

`node`  

The audio node with the inputs you want to disconnect.

## Discussion

Connections break on each of the audio node’s input buses.

## See Also

### Connecting and Disconnecting Audio Nodes

func connect(AVAudioNode, to: AVAudioNode, format: AVAudioFormat?)

Establishes a connection between two nodes.

func connect(AVAudioNode, to: AVAudioNode, fromBus: AVAudioNodeBus, toBus: AVAudioNodeBus, format: AVAudioFormat?)

Establishes a connection between two nodes, specifying the input and output busses.

func disconnectNodeInput(AVAudioNode, bus: AVAudioNodeBus)

Removes the input connection of a node on the specified bus.

func disconnectNodeOutput(AVAudioNode)

Removes all output connections of a node.

func disconnectNodeOutput(AVAudioNode, bus: AVAudioNodeBus)

Removes the output connection of a node on the specified bus.

