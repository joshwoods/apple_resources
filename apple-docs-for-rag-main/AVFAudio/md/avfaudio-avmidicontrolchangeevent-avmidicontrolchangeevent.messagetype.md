

- AVFAudio
- AVMIDIControlChangeEvent
-  AVMIDIControlChangeEvent.MessageType 

Enumeration

# AVMIDIControlChangeEvent.MessageType

Constants that represents control change event types.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum MessageType
```

## Topics

### Event Types

case bankSelect

An event type for switching bank selection.

case modWheel

An event type for modulating a vibrato effect.

case breath

An event type for a breath controller.

case foot

An event type for sending continuous stream of values when using a foot controller.

case portamentoTime

An event type for controlling the portamento rate.

case dataEntry

An event type for controlling the data entry parameters.

case volume

An event type for controlling the channel volume.

case balance

An event type for controlling the left and right channel balance.

case pan

An event type for controlling the left and right channel pan.

case expression

An event type that represents an expression controller.

case sustain

An event type for switching a damper pedal on or off.

case portamento

An event type for switching portamento on or off.

case sostenuto

An event type for switching sostenuto on or off.

case soft

An event type for lowering the volume of the notes.

case legatoPedal

An event type for switching the legato pedal on or off.

case hold2Pedal

An event type for holding notes.

case filterResonance

An event type for a filter resonance.

case releaseTime

An event type for controlling the release time.

case attackTime

An event type for controlling the attack time.

case brightness

An event type for controlling the brightness.

case decayTime

An event type for controlling the decay time.

case vibratoRate

An event type for controlling the vibrato rate.

case vibratoDepth

An event type for controlling the vibrato depth.

case vibratoDelay

An event type for controlling the vibrato delay.

case reverbLevel

An event type for controlling the reverb level.

case chorusLevel

An event type for controlling the chorus level.

case RPN_LSB

An event type that represents the registered parameter number LSB.

case RPN_MSB

An event type that represents the registered parameter number MSB.

case allSoundOff

An event type for muting all sounding notes.

case resetAllControllers

An event type for resetting all controllers to their default state.

case allNotesOff

An event type for muting all sounding notes while maintaining the release time.

case omniModeOff

An event type for setting omni off mode.

case omniModeOn

An event type for setting omni on mode.

case monoModeOn

An event type for setting the device mode to monophonic.

case monoModeOff

An event type for setting the device mode to polyphonic.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting a Control Change Event

var value: UInt32

The value of the control change event.

var messageType: AVMIDIControlChangeEvent.MessageType

The type of control change message.

