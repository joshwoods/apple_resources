

- Audio Toolbox
-  AUParameterEvent 

Structure

# AUParameterEvent

A structure that describes a scheduled parameter event.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AUParameterEvent
```

## Topics

### Initializers

init()

init(next: UnsafeMutablePointer&lt;AURenderEvent>?, eventSampleTime: AUEventSampleTime, eventType: AURenderEventType, reserved: (UInt8, UInt8, UInt8), rampDurationSampleFrames: AUAudioFrameCount, parameterAddress: AUParameterAddress, value: AUValue)

### Instance Properties

var eventSampleTime: AUEventSampleTime

The sample time at which the event is scheduled to occur.

var eventType: AURenderEventType

The type of render event. Must be AURenderEventType.parameter or AURenderEventType.parameterRamp.

var next: UnsafeMutablePointer&lt;AURenderEvent>?

The next event in a linked list of events.

var parameterAddress: AUParameterAddress

The parameter to change.

var rampDurationSampleFrames: AUAudioFrameCount

The ramp duration, in sample frames. Must be `0` for a non-ramped event; otherwise, must be greater than `0` for a ramped event.

var reserved: (UInt8, UInt8, UInt8)

Reserved field. Must be `0`.

var value: AUValue

For a non-ramped event, this is the new parameter value. For a ramped event, this is the parameter value at the end of the ramp.

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

