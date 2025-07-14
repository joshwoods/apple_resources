

- Audio Toolbox
-  AUSamplerBankPresetData 

Structure

# AUSamplerBankPresetData

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AUSamplerBankPresetData
```

## Topics

### Initializers

init(bankURL: Unmanaged&lt;CFURL>, bankMSB: UInt8, bankLSB: UInt8, presetID: UInt8, reserved: UInt8)

### Instance Properties

var bankLSB: UInt8

var bankMSB: UInt8

var bankURL: Unmanaged&lt;CFURL>

var presetID: UInt8

var reserved: UInt8

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

