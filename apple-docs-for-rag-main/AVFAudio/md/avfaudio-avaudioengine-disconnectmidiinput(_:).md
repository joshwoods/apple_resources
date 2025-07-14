

- AVFAudio
- AVAudioEngine
-  disconnectMIDIInput(\_:) 

Instance Method

# disconnectMIDIInput(\_:)

Disconnects all input MIDI connections from a node.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func disconnectMIDIInput(_ node: AVAudioNode)
```

## Parameters 

`node`  

The node with the MIDI input to disconnect.

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

func disconnectMIDIOutput(AVAudioNode)

Disconnects all output MIDI connections from a node.

func connectMIDI(AVAudioNode, to: AVAudioNode, format: AVAudioFormat?, block: AUMIDIOutputEventBlock?)

Establishes a MIDI-only connection between two nodes.

Deprecated

func connectMIDI(AVAudioNode, to: [AVAudioNode], format: AVAudioFormat?, block: AUMIDIOutputEventBlock?)

Establishes a MIDI-only connection between a source node and multiple destination nodes.

Deprecated

