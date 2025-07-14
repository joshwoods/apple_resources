

- Audio Toolbox
-  AudioUnitParameterInfo 

Structure

# AudioUnitParameterInfo

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioUnitParameterInfo
```

## Topics

### Initializers

init()

init(name: (CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar), unitName: Unmanaged&lt;CFString>?, clumpID: UInt32, cfNameString: Unmanaged&lt;CFString>?, unit: AudioUnitParameterUnit, minValue: AudioUnitParameterValue, maxValue: AudioUnitParameterValue, defaultValue: AudioUnitParameterValue, flags: AudioUnitParameterOptions)

### Instance Properties

var cfNameString: Unmanaged&lt;CFString>?

Only valid if `kAudioUnitParameterFlag_HasCFNameString` is set.

var clumpID: UInt32

Only valid if `kAudioUnitParameterFlag_HasClump` is set.

var defaultValue: AudioUnitParameterValue

var flags: AudioUnitParameterOptions

The host should check for this flag and, if present, release the parameter name when it is finished with it.

var maxValue: AudioUnitParameterValue

var minValue: AudioUnitParameterValue

var name: (CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar)

Must be set to `0`.

var unit: AudioUnitParameterUnit

If the `unit` field contains a value not in the `AudioUnitParameterUnit` enumeration, then assume the unit type is `kAudioUnitParameterUnit_Generic`.

var unitName: Unmanaged&lt;CFString>?

If `kAudioUnitParameterUnit_CustomUnit` is set, this field must contain a valid `CFString` object. Only valid if `kAudioUnitParameterUnit_CustomUnit` is set.

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

struct AudioUnitParameterOptions

Value options for audio unit parameters.

struct AudioUnitParameterStringFromValue

A string representation of a parameter’s value.

struct AudioUnitParameterValueFromString

A parameter’s value based on a string representation of the value.

