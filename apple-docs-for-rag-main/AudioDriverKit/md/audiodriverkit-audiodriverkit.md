

- AudioDriverKit
-  AudioDriverKit 

Namespace

# AudioDriverKit

DriverKit 21.0+

``` source
namespace AudioDriverKit;
```

## Topics

### Structures

IOUserAudioCustomPropertyInfo

A description of a custom property’s data types.

IOUserAudioObjectPropertyAddress

An object that collects the three parts — selector, scope, and element — that identify a specific property.

IOUserAudioStreamBasicDescription

A structure that encapsulates all of the information for describing the basic format properties of a stream of audio data.

### Variables

IOUserAudioIOOperationBeginRead

IOUserAudioIOOperationWriteEnd

IOUserAudioObjectPropertyElementMain

The identifier for an audio object’s main element.

kIOUserAudioObjectIDDriver

The audio object ID of the driver.

### Type Aliases

IOOperationHandler

IOUserAudioIOOperation

IOUserAudioObjectID

An identifier that provides a handle on a specific audio object.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertySelector

A four character code which, along with the scope and element, specific piece of information about an audio object.

### Enumerations

IOUserAudioChannelLabel

Constants to set the preferred channel layout on an audio device.

IOUserAudioClassID

An identifier for the type of audio object.

IOUserAudioClockAlgorithm

Values that describe clock-smoothing algorithms.

IOUserAudioCustomPropertyDataType

A data and qualifier type used for custom properties.

IOUserAudioDeviceTransportState

IOUserAudioFormatFlags

Flag values that provide more information about the format used by an audio stream basic description.

IOUserAudioFormatID

An enumeration of four character codes used to identify distinct audio data formats.

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

IOUserAudioReservedConfigChangeAction

Identifiers for object state changes that require a configuration change.

IOUserAudioStartStopFlags

Values that indicate I/O starts or stops.

IOUserAudioStreamDirection

A type representing the direction of audio flow.

IOUserAudioStreamTerminalType

Constants that describe the terminal type of an audio stream.

IOUserAudioTransportType

The type of transport to deliver audio.

