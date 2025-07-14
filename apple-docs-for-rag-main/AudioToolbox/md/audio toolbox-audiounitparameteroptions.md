

- Audio Toolbox
-  AudioUnitParameterOptions 

Structure

# AudioUnitParameterOptions

Value options for audio unit parameters.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioUnitParameterOptions
```

## Overview

These constants are relevant only in macOS, and not in iOS.

Audio unit parameter flags, for use in the AudioUnitParameterInfo data structure , serve as a dictionary-like set of information about an audio unit parameter. Parameter flag bit position 19 is reserved.

## Topics

### Constants

static var flag_CFNameRelease: AudioUnitParameterOptions

If an audio unit can generate parameter names dynamically, it should set this flag.

static var flag_CanRamp: AudioUnitParameterOptions

static var flag_DisplayCubeRoot: AudioUnitParameterOptions

static var flag_DisplayCubed: AudioUnitParameterOptions

static var flag_DisplayExponential: AudioUnitParameterOptions

static var flag_DisplayLogarithmic: AudioUnitParameterOptions

static var flag_DisplayMask: AudioUnitParameterOptions

static var flag_DisplaySquareRoot: AudioUnitParameterOptions

static var flag_DisplaySquared: AudioUnitParameterOptions

static var flag_ExpertMode: AudioUnitParameterOptions

static var flag_HasCFNameString: AudioUnitParameterOptions

static var flag_HasClump: AudioUnitParameterOptions

static var flag_IsElementMeta: AudioUnitParameterOptions

static var flag_IsGlobalMeta: AudioUnitParameterOptions

static var flag_IsHighResolution: AudioUnitParameterOptions

static var flag_IsReadable: AudioUnitParameterOptions

static var flag_IsWritable: AudioUnitParameterOptions

static var flag_MeterReadOnly: AudioUnitParameterOptions

static var flag_NonRealTime: AudioUnitParameterOptions

static var flag_OmitFromPresets: AudioUnitParameterOptions

static var flag_PlotHistory: AudioUnitParameterOptions

If set, getting the `kAudioUnitProperty_ParameterHistoryInfo` property fills out the AudioUnitParameterHistoryInfo struct containing the recommended update rate and history duration.

static var flag_ValuesHaveStrings: AudioUnitParameterOptions

### Initializers

init(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

struct AudioUnitParameterStringFromValue

A string representation of a parameter’s value.

struct AudioUnitParameterValueFromString

A parameter’s value based on a string representation of the value.

