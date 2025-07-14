

- AVFAudio
- AVAudioEngine
-  connectMIDI(\_:to:format:block:) Deprecated

Instance Method

# connectMIDI(\_:to:format:block:)

Establishes a MIDI-only connection between a source node and multiple destination nodes.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.14–13.0DeprecatedtvOS 12.0–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func connectMIDI(
    _ sourceNode: AVAudioNode,
    to destinationNodes: [AVAudioNode],
    format: AVAudioFormat?,
    block tapBlock: AUMIDIOutputEventBlock? = nil
)
```

Deprecated

Use connectMIDI(_:to:format:eventListBlock:) instead.

## Parameters 

`sourceNode`  

The source node.

`destinationNodes`  

An array of AVAudioNode objects that specify destination nodes.

`format`  

If not `NULL`, the engine uses this value for the format of the source audio node’s output bus. In all cases, the format of the source node’s output bus has to match with the destination node’s output bus format.

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

func connectMIDI(AVAudioNode, to: AVAudioNode, format: AVAudioFormat?, block: AUMIDIOutputEventBlock?)

Establishes a MIDI-only connection between two nodes.

Deprecated

