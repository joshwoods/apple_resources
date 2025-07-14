

- Audio Toolbox
-  AURenderEventHeader 

Structure

# AURenderEventHeader

The common header for a render event.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AURenderEventHeader
```

## Topics

### Initializers

init()

init(next: UnsafeMutablePointer&lt;AURenderEvent>?, eventSampleTime: AUEventSampleTime, eventType: AURenderEventType, reserved: UInt8)

### Instance Properties

var eventSampleTime: AUEventSampleTime

The sample time at which the event is scheduled to occur.

var eventType: AURenderEventType

The type of the event.

var next: UnsafeMutablePointer&lt;AURenderEvent>?

The next event in a linked list of events.

var reserved: UInt8

Reserved field. Must be `0`.

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

