

- Audio Toolbox
- AUAudioUnit
-  isMusicDeviceOrEffect 

Instance Property

# isMusicDeviceOrEffect

Specifies whether an audio unit responds to MIDI events.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var isMusicDeviceOrEffect: Bool { get }
```

## Discussion

Returns true if the audio unit is a music device or effect.

## See Also

### Managing MIDI Events

var virtualMIDICableCount: Int

The number of virtual MIDI cables implemented by a music device or effect.

var scheduleMIDIEventBlock: AUScheduleMIDIEventBlock?

A block used to schedule MIDI events.

var midiOutputEventBlock: AUMIDIOutputEventBlock?

var midiOutputNames: [String]

The names of the MIDI outputs.

typealias AUScheduleMIDIEventBlock

A block to schedule MIDI events.

typealias AUMIDIOutputEventBlock

