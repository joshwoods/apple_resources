

- Audio Toolbox
- AUAudioUnit
-  midiOutputNames 

Instance Property

# midiOutputNames

The names of the MIDI outputs.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var midiOutputNames: [String] { get }
```

## See Also

### Managing MIDI Events

var isMusicDeviceOrEffect: Bool

Specifies whether an audio unit responds to MIDI events.

var virtualMIDICableCount: Int

The number of virtual MIDI cables implemented by a music device or effect.

var scheduleMIDIEventBlock: AUScheduleMIDIEventBlock?

A block used to schedule MIDI events.

var midiOutputEventBlock: AUMIDIOutputEventBlock?

typealias AUScheduleMIDIEventBlock

A block to schedule MIDI events.

typealias AUMIDIOutputEventBlock

