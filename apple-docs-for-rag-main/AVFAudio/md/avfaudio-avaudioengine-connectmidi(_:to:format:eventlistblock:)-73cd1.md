

- AVFAudio
- AVAudioEngine
-  connectMIDI(\_:to:format:eventListBlock:) 

Instance Method

# connectMIDI(\_:to:format:eventListBlock:)

Establishes a MIDI connection between two nodes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func connectMIDI(
    _ sourceNode: AVAudioNode,
    to destinationNode: AVAudioNode,
    format: AVAudioFormat?,
    eventListBlock tapBlock: AUMIDIEventListBlock? = nil
)
```

## Parameters 

`sourceNode`  

The source node.

`destinationNode`  

The destination node.

`format`  

If not `NULL`, the engine uses this value for the format of the source audio node’s output bus. In all cases, the engine matches the format of the destination audio node’s input bus to the source node’s output bus.

`tapBlock`  

If not `NULL`, the source node’s event list block calls this on the real-time thread. The host can tap the MIDI data of the source node through this block.

## Discussion

Use this to establish a MIDI connection between a source node and a destination node that has MIDI input capability. This method disconnects any existing MIDI connection that involves the destination node. When making the MIDI connection, this method overwrites the source node’s event list block.

The source node can only be an AVAudioUnit node with the type kAudioUnitType_MIDIProcessor. The destination node types can be kAudioUnitType_MusicDevice, kAudioUnitType_MusicEffect, or kAudioUnitType_MIDIProcessor.

## See Also

### Managing MIDI Nodes

func connectMIDI(AVAudioNode, to: [AVAudioNode], format: AVAudioFormat?, eventListBlock: AUMIDIEventListBlock?)

Establishes a MIDI connection between a source node and multiple destination nodes.

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

