

- Audio Toolbox
- Deprecated Symbols
-  Audio Unit Processing Graph Services 

API Collection

# Audio Unit Processing Graph Services

Audio Unit Processing Graph Services provide interfaces for representing a set of audio units, connections between their inputs and outputs, and callbacks used to provide inputs. It also enables the embedding of sub (or child) processing graphs within parent graphs to allow for a logical organization of parts of an overall signal chain.

## Overview

An audio processing graph object (of type `AUGraph`) is a complete description of an audio signal processing network. Audio Unit Processing Graph Services may manage the instantiated audio units if the `AUGraphOpen` function is called.

An audio processing graph object may be introspected to get complete information about all of the audio units in the graph. The various node objects (each of type `AUNode`) in the graph, each representing an audio unit or a sub graph, may be added or removed, and the interactions between them modified.

A graph object’s state can be manipulated in both the rendering thread and in other threads. Consequently, any activities that affect the state of the graph are guarded with locks and a messaging model between any calling thread and the thread upon which the graph object’s output unit is called (the render thread).

A graph object will have a single head node––an output unit. The output unit is used to both start and stop the rendering operations of a graph, and is the dispatch point for the safe manipulation of the state of the graph while it is running.

## Topics

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

func AUGraphInitialize(AUGraph) -> OSStatus

Initializes an audio processing graph.

Deprecated

func AUGraphIsInitialized(AUGraph, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Determines whether an audio processing graph is initialized.

Deprecated

func AUGraphIsNodeSubGraph(AUGraph, AUNode, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Determines whether a node object represent an audio processing graph or an audio unit.

Deprecated

func AUGraphIsOpen(AUGraph, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Determines whether an audio processing graph is open.

Deprecated

func AUGraphIsRunning(AUGraph, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Determines whether an audio processing graph running.

Deprecated

func AUGraphNewNodeSubGraph(AUGraph, UnsafeMutablePointer&lt;AUNode>) -> OSStatus

Creates a node object to represent a subgraph.

Deprecated

func AUGraphNodeInfo(AUGraph, AUNode, UnsafeMutablePointer&lt;AudioComponentDescription>?, UnsafeMutablePointer&lt;AudioUnit?>?) -> OSStatus

Returns information about a node object.

Deprecated

func AUGraphOpen(AUGraph) -> OSStatus

Opens an audio processing graph.

Deprecated

func AUGraphRemoveNode(AUGraph, AUNode) -> OSStatus

Removes a node from an audio processing graph.

Deprecated

func AUGraphRemoveRenderNotify(AUGraph, AURenderCallback, UnsafeMutableRawPointer?) -> OSStatus

Removes a notification callback from an audio processing graph.

Deprecated

func AUGraphSetNodeInputCallback(AUGraph, AUNode, UInt32, UnsafePointer&lt;AURenderCallbackStruct>) -> OSStatus

Sets an input callback function for a node.

Deprecated

func AUGraphStart(AUGraph) -> OSStatus

Starts an audio processing graph.

Deprecated

func AUGraphStop(AUGraph) -> OSStatus

Stops an audio processing graph.

Deprecated

func AUGraphUninitialize(AUGraph) -> OSStatus

Uninitializes an audio processing graph.

Deprecated

func AUGraphUpdate(AUGraph, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Updates the state of a running audio processing graph.

Deprecated

func DisposeAUGraph(AUGraph) -> OSStatus

Disposes of an audio processing graph.

Deprecated

func NewAUGraph(UnsafeMutablePointer&lt;AUGraph?>) -> OSStatus

Creates a new audio processing graph.

Deprecated

### Data Types

struct AudioUnitNodeConnection

A connection between two node objects in an audio processing graph.

typealias AUGraph

An opaque type representing an audio processing graph.

typealias AUNode

A member of an audio processing graph, associated with an audio unit.

struct AUNodeInteraction

Describes the interaction between two node objects.

struct AUNodeRenderCallback

A callback used to provide input to an audio unit.

### Constants

kAUNodeInteraction_Connection

The different types of node interactions.

### Result Codes

This table lists the result codes defined for Audio Unit Processing Graph Services.

var kAUGraphErr_NodeNotFound: OSStatus

The specified node cannot be found.

var kAUGraphErr_InvalidConnection: OSStatus

The attempted connection between two nodes cannot be made.

var kAUGraphErr_OutputNodeErr: OSStatus

Audio processing graphs can only contain one output unit. This error is returned if trying to add a second output unit or if the graph’s output unit is removed while the graph is running.

var kAUGraphErr_CannotDoInCurrentContext: OSStatus

To avoid spinning or waiting in the render thread (a bad idea!), many of the calls to AUGraph can return: `kAUGraphErr_CannotDoInCurrentContext`. This result is only generated when you call an AUGraph API from its render callback. It means that the lock that it required was held at that time, by another thread. If you see this result code, you can generally attempt the action again - typically the NEXT render cycle (so in the mean time the lock can be cleared), or you can delegate that call to another thread in your app. You should not spin or put-to-sleep the render thread.

var kAUGraphErr_InvalidAudioUnit: OSStatus

