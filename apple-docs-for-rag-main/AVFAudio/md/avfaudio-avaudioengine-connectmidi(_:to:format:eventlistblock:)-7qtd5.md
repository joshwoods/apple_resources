

- AVFAudio
- AVAudioEngine
-  connectMIDI(\_:to:format:eventListBlock:) 

Instance Method

# connectMIDI(\_:to:format:eventListBlock:)

Establishes a MIDI connection between a source node and multiple destination nodes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func connectMIDI(
    _ sourceNode: AVAudioNode,
    to destinationNodes: [AVAudioNode],
    format: AVAudioFormat?,
    eventListBlock tapBlock: AUMIDIEventListBlock? = nil
)
```

## Parameters 

`sourceNode`  

The source node.

`destinationNodes`  

An array of objects that specify the destination nodes.

`format`  

If not `NULL`, the engine uses this value for the format of the source audio node’s output bus. In all cases, the format of the source node’s output bus has to match with the destination node’s output bus format.

`tapBlock`  

If not `NULL`, the source node’s event list block calls this on the real-time thread. The host can tap the MIDI data of the source node through this block.

## Discussion

Use this to establish a MIDI connection between a source node and multiple destination nodes that have MIDI input capability. This method disconnects any existing MIDI connection that involves the destination node. When making the MIDI connection, this method overwrites the source node’s event list block.

The source node can only be an AVAudioUnit node with the type kAudioUnitType_MIDIProcessor. The destination node types can be kAudioUnitType_MusicDevice, kAudioUnitType_MusicEffect, or kAudioUnitType_MIDIProcessor.

MIDI connections made with this method specify a single destination connection (one-to-one) or multiple connections (one-to-many), but never many-to-one.

## See Also

### Managing MIDI Nodes

func connectMIDI(AVAudioNode, to: AVAudioNode, format: AVAudioFormat?, eventListBlock: AUMIDIEventListBlock?)

Establishes a MIDI connection between two nodes.

func disconnectMIDI(AVAudioNode, from: AVAudioNode)

Removes a MIDI connection between two nodes.

func disconnectMIDI(AVAudioNode, from: [AVAudioNode])

Removes a MIDI connection between one source node and multiple destination nodes.

func disconnectMIDIInput(AVAudioNode)

Disconnects all input MIDI connections from a node.

func disconnectMIDIOutput(AVAudioNode)

Disconnects all output MIDI connections from a node.

func connectMIDI(AVAudioNode, to: AVAudioNode, format: AVAudioFormat?, block: AUMIDIOutputEventBlock?)

Establishes a MIDI-only connection between two nodes.

Deprecated

func connectMIDI(AVAudioNode, to: [AVAudioNode], format: AVAudioFormat?, block: AUMIDIOutputEventBlock?)

Establishes a MIDI-only connection between a source node and multiple destination nodes.

Deprecated

