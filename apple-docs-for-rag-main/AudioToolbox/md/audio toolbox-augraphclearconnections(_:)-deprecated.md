

- Audio Toolbox
-  AUGraphClearConnections(\_:) Deprecated

Function

# AUGraphClearConnections(\_:)

Clears all of the interactions in an audio unit processing graph.

iOS 2.0–14.0DeprecatediPadOS 2.0–14.0DeprecatedMac Catalyst 13.1+macOS 10.0–11.0DeprecatedtvOS 9.0+visionOS 1.0+

``` source
func AUGraphClearConnections(_ inGraph: AUGraph) -> OSStatus
```

Deprecated

AUGraph is deprecated in favor of AVAudioEngine

## Parameters 

`inGraph`  

## Return Value

## Discussion

This will clear all connections and callback interactions of the nodes of a graph.

## See Also

### Audio Unit Processing Graph Services Functions

func AUGraphAddNode(AUGraph, UnsafePointer&lt;AudioComponentDescription>, UnsafeMutablePointer&lt;AUNode>) -> OSStatus

Adds a node to an audio processing graph.

Deprecated

func AUGraphAddRenderNotify(AUGraph, AURenderCallback, UnsafeMutableRawPointer?) -> OSStatus

Adds a render notification callback to an audio processing graph.

Deprecated

func AUGraphClose(AUGraph) -> OSStatus

Closes an audio unit processing graph.

Deprecated

func AUGraphConnectNodeInput(AUGraph, AUNode, UInt32, AUNode, UInt32) -> OSStatus

Connects one node’s output to another node’s input.

Deprecated

func AUGraphCountNodeInteractions(AUGraph, AUNode, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Retrieves the number of interactions of an audio processing graph’s node.

Deprecated

func AUGraphDisconnectNodeInput(AUGraph, AUNode, UInt32) -> OSStatus

Disconnects a node’s input.

Deprecated

func AUGraphGetCPULoad(AUGraph, UnsafeMutablePointer&lt;Float32>) -> OSStatus

Obtains the short-term running average of the current CPU load of the audio processing graph.

Deprecated

func AUGraphGetIndNode(AUGraph, UInt32, UnsafeMutablePointer&lt;AUNode>) -> OSStatus

Gets the audio processing graph node at a given index.

Deprecated

func AUGraphGetInteractionInfo(AUGraph, UInt32, UnsafeMutablePointer&lt;AUNodeInteraction>) -> OSStatus

Retrieves information about a particular interaction in an audio processing graph.

Deprecated

func AUGraphGetMaxCPULoad(AUGraph, UnsafeMutablePointer&lt;Float32>) -> OSStatus

Obtains the maximum CPU load of an audio processing graph since this call was last made or since the graph was last started.

Deprecated

func AUGraphGetNodeCount(AUGraph, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

The number of nodes in an audio processing graph.

Deprecated

func AUGraphGetNodeInfoSubGraph(AUGraph, AUNode, UnsafeMutablePointer&lt;AUGraph?>) -> OSStatus

Gets the audio processing subgraph object represented by a node.

Deprecated

func AUGraphGetNodeInteractions(AUGraph, AUNode, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AUNodeInteraction>) -> OSStatus

Retrieves information about the interactions in an audio processing graph for a given node.

Deprecated

func AUGraphGetNumberOfInteractions(AUGraph, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Retrieves the number of interactions for an audio processing graph.

Deprecated

func AUGraphInitialize(AUGraph) -> OSStatus

Initializes an audio processing graph.

Deprecated

