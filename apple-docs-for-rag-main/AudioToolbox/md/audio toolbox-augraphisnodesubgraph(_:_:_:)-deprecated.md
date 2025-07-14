

- Audio Toolbox
-  AUGraphIsNodeSubGraph(\_:\_:\_:) Deprecated

Function

# AUGraphIsNodeSubGraph(\_:\_:\_:)

Determines whether a node object represent an audio processing graph or an audio unit.

macOS 10.2–11.0Deprecated

``` source
func AUGraphIsNodeSubGraph(
    _ inGraph: AUGraph,
    _ inNode: AUNode,
    _ outFlag: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

no longer supported

## Parameters 

`inGraph`  

The `AUGraph` object containing the node you want to query.

`inNode`  

The node to query.

`outFlag`  

On output, true if the node is a subgraph, false if not.

## Return Value

A result code.

## Discussion

## See Also

### Audio Unit Processing Graph Services Functions

func AUGraphAddNode(AUGraph, UnsafePointer&lt;AudioComponentDescription>, UnsafeMutablePointer&lt;AUNode>) -> OSStatus

Adds a node to an audio processing graph.

Deprecated

func AUGraphAddRenderNotify(AUGraph, AURenderCallback, UnsafeMutableRawPointer?) -> OSStatus

Adds a render notification callback to an audio processing graph.

Deprecated

func AUGraphClearConnections(AUGraph) -> OSStatus

Clears all of the interactions in an audio unit processing graph.

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

