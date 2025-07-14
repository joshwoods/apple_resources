

- Audio Toolbox
-  AudioUnitParameterStringFromValue 

Structure

# AudioUnitParameterStringFromValue

A string representation of a parameter’s value.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioUnitParameterStringFromValue
```

## Topics

### Initializers

init(inParamID: AudioUnitParameterID, inValue: UnsafePointer&lt;AudioUnitParameterValue>, outString: Unmanaged&lt;CFString>?)

### Instance Properties

var inParamID: AudioUnitParameterID

var inValue: UnsafePointer&lt;AudioUnitParameterValue>

var outString: Unmanaged&lt;CFString>?

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

struct AudioUnitParameterValueFromString

A parameter’s value based on a string representation of the value.

