

- Audio Toolbox
-  AURenderEvent 

Structure

# AURenderEvent

A union of the various specific render event types.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AURenderEvent
```

## Topics

### Instance Properties

var MIDI: AUMIDIEvent

Use this field for MIDI events.

var head: AURenderEventHeader

Use this field to determine the event type.

var parameter: AUParameterEvent

Use this field for parameter events.

var MIDIEventsList: AUMIDIEventList

### Initializers

init()

init(MIDI: AUMIDIEvent)

init(MIDIEventsList: AUMIDIEventList)

init(head: AURenderEventHeader)

init(parameter: AUParameterEvent)

## Relationships

### Conforms To

- Sendable

## See Also

### Structures

struct AudioUnitConnection

An audio unit source-to-destination connection specification.

struct AudioUnitEvent

struct AudioUnitExternalBuffer

Allows an audio unit host application to tell an audio unit to use a specified buffer for its input callback.

struct AudioUnitFrequencyResponseBin

An audio unit’s audio level at a particular frequency.

struct AudioUnitMeterClipping

Audio clipping that has occurred in a mixer unit.

struct AudioUnitMIDIControlMapping

struct AudioUnitOtherPluginDesc

struct AudioUnitParameter

An adjustable audio unit attribute such as volume, pitch, or filter cutoff frequency.

struct AudioUnitParameterEvent

A scheduled change to an audio unit parameter’s value.

struct AudioUnitParameterHistoryInfo

The suggested update rate and history duration for parameters which have the flag_PlotHistory flag set.

struct AudioUnitParameterNameInfo

A short version of the name for an audio unit parameter.

typealias AudioUnitParameterIDName

A type definition for a data type that defines the short version of the name for an audio unit parameter.

struct AudioUnitParameterInfo

struct AudioUnitParameterOptions

Value options for audio unit parameters.

struct AudioUnitParameterStringFromValue

A string representation of a parameter’s value.

