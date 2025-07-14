

- AVFAudio
- AVAudioEngine
-  connectMIDI(\_:to:format:block:) Deprecated

Instance Method

# connectMIDI(\_:to:format:block:)

Establishes a MIDI-only connection between two nodes.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.14–13.0DeprecatedtvOS 12.0–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func connectMIDI(
    _ sourceNode: AVAudioNode,
    to destinationNode: AVAudioNode,
    format: AVAudioFormat?,
    block tapBlock: AUMIDIOutputEventBlock? = nil
)
```

Deprecated

Use connectMIDI(_:to:format:eventListBlock:) instead.

## Parameters 

`sourceNode`  

The source node.

`destinationNode`  

The destination node.

`format`  

If not `NULL`, the engine uses this value for the format of the source audio node’s output bus. In all cases, the engine matches the format of the destination audio node’s input bus to the source audio node’s output bus.

`tapBlock`  

If not `NULL`, the source node’s AUMIDIOutputEventBlock calls this block on the real-time thread. The host can tap the MIDI data of the source node through this block.

## See Also

### Managing MIDI Nodes

func connectMIDI(AVAudioNode, to: AVAudioNode, format: AVAudioFormat?, eventListBlock: AUMIDIEventListBlock?)

Establishes a MIDI connection between two nodes.

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

func connectMIDI(AVAudioNode, to: [AVAudioNode], format: AVAudioFormat?, block: AUMIDIOutputEventBlock?)

Establishes a MIDI-only connection between a source node and multiple destination nodes.

Deprecated

