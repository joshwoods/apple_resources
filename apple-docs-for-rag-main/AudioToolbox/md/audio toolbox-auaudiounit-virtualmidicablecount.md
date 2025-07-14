

- Audio Toolbox
- AUAudioUnit
-  virtualMIDICableCount 

Instance Property

# virtualMIDICableCount

The number of virtual MIDI cables implemented by a music device or effect.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var virtualMIDICableCount: Int { get }
```

## Discussion

A music device or effect can support up to 256 virtual MIDI cables of input.

## See Also

### Managing MIDI Events

var isMusicDeviceOrEffect: Bool

Specifies whether an audio unit responds to MIDI events.

var scheduleMIDIEventBlock: AUScheduleMIDIEventBlock?

A block used to schedule MIDI events.

var midiOutputEventBlock: AUMIDIOutputEventBlock?

var midiOutputNames: [String]

The names of the MIDI outputs.

typealias AUScheduleMIDIEventBlock

A block to schedule MIDI events.

typealias AUMIDIOutputEventBlock

