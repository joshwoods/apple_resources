

- Audio Toolbox
-  AUMIDIOutputCallbackStruct 

Structure

# AUMIDIOutputCallbackStruct

The callback function and custom data for an audio unit that provides MIDI output.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AUMIDIOutputCallbackStruct
```

## Topics

### Initializers

init(midiOutputCallback: AUMIDIOutputCallback, userData: UnsafeMutableRawPointer?)

### Instance Properties

var midiOutputCallback: AUMIDIOutputCallback

The callback function for an audio unit that provides MIDI output.

var userData: UnsafeMutableRawPointer?

Custom data for an audio unit that provides MIDI output.

## Relationships

### Conforms To

- BitwiseCopyable

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

