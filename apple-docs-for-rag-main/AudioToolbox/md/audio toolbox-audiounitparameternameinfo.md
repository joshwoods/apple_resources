

- Audio Toolbox
-  AudioUnitParameterNameInfo 

Structure

# AudioUnitParameterNameInfo

A short version of the name for an audio unit parameter.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioUnitParameterNameInfo
```

## Discussion

This data structure is used as a value for the kAudioUnitProperty_ParameterClumpName and kAudioUnitProperty_ParameterIDName audio unit properties.

## Topics

### Initializers

init()

init(inID: AudioUnitParameterID, inDesiredLength: Int32, outName: Unmanaged&lt;CFString>?)

### Instance Properties

var inDesiredLength: Int32

When setting an audio unit property that uses this data structure for its value, the maximum length that you are specifying for the audio unit parameter name.

var inID: AudioUnitParameterID

The identifier for the audio unit parameter.

var outName: Unmanaged&lt;CFString>?

When getting an audio unit property that uses this data structure for its value, the short version of the parameter name provided by the audio unit. The host application then owns the string and is responsible for releasing it.

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

typealias AudioUnitParameterIDName

A type definition for a data type that defines the short version of the name for an audio unit parameter.

struct AudioUnitParameterInfo

struct AudioUnitParameterOptions

Value options for audio unit parameters.

struct AudioUnitParameterStringFromValue

A string representation of a parameter’s value.

struct AudioUnitParameterValueFromString

A parameter’s value based on a string representation of the value.

