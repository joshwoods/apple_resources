

- Audio Toolbox
-  AUGraphUpdate(\_:\_:) Deprecated

Function

# AUGraphUpdate(\_:\_:)

Updates the state of a running audio processing graph.

iOS 2.0–14.0DeprecatediPadOS 2.0–14.0DeprecatedMac Catalyst 13.1+macOS 10.0–11.0DeprecatedtvOS 9.0+visionOS 1.0+

``` source
func AUGraphUpdate(
    _ inGraph: AUGraph,
    _ outIsUpdated: UnsafeMutablePointer?
) -> OSStatus
```

Deprecated

AUGraph is deprecated in favor of AVAudioEngine

## Parameters 

`inGraph`  

`outIsUpdated`  

In input, pass `NULL` for synchronous (blocking) behavior, or non-`NULL` to have this function return immediately. On output, `true` if all of the edits were applied to the audio processing graph at the time of function return.

## Return Value

A result code.

## Discussion

Call this function to finalize changes to an audio processing graph’s state after making calls such as AUGraphConnectNodeInput(_:_:_:_:_:).

Node connections and disconnections can be completely processed in the render notification callback of a graph, finalized by calling this function from within the callback. You can also remove nodes (apart from the head node) from within the render notification callback.

If this function returns the `kAUGraphErr_CannotDoInCurrentContext` result code, another thread was calling a function dependent on the graph’s existing state. When the competing thread completes its call, call this function again.

Audio processing graph updates are all or none. If this function encounters any errors while attempting to finalize graph events, then no pending changes are finalized.

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

