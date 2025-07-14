

- Audio Toolbox
-  AUAudioUnitBus 

Class

# AUAudioUnitBus

A class that defines an input or output connection point on an audio unit.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class AUAudioUnitBus
```

## Topics

### Bus Methods and Properties

func setFormat(AVAudioFormat) throws

Sets the bus’s audio format.

var format: AVAudioFormat

The audio format and channel layout of audio being transferred on the bus.

var isEnabled: Bool

Determines whether the bus is active.

var name: String?

A name for the bus.

var index: Int

The index of this bus in its containing array.

var busType: AUAudioUnitBusType

The bus type.

var ownerAudioUnit: AUAudioUnit

The audio unit that owns the bus.

var supportedChannelLayoutTags: [NSNumber]?

An array of audio channel layout tags.

var contextPresentationLatency: TimeInterval

Information about latency in the audio unit’s processing context.

var shouldAllocateBuffer: Bool

### Audio Unit Implementations

These methods and properties are only of interest to audio unit subclasses.

init(format: AVAudioFormat) throws

Initializes a bus object with a specific format.

var supportedChannelCounts: [NSNumber]?

An array of numbers indicating the supported number of channels for this bus.

var maximumChannelCount: AUAudioChannelCount

The maximum number of channels supported for this bus.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio Units

Creating an audio unit extension

Build an extension by using an Xcode template.

Creating custom audio effects

Add custom audio-effect processing to apps like Logic Pro X and GarageBand by creating Audio Unit (AU) plug-ins.

Incorporating Audio Effects and Instruments

Add custom audio processing and MIDI instruments to your app by hosting Audio Unit (AU) plug-ins.

Debugging Out-of-Process Audio Units on Apple Silicon

Connect to out-of-process audio units using the Xcode debugger.

class AUAudioUnit

A class that defines a host’s interface to an audio unit.

class AUAudioUnitBusArray

A class that defines a container for an audio unit’s input or output busses.

class AUAudioUnitPreset

A class that describes an interface for custom parameter settings provided by the audio unit developer.

class AUAudioUnitV2Bridge

A class that wraps a version 2 audio unit as version 3 audio unit.

func AudioUnitExtensionCopyComponentList(CFString) -> Unmanaged&lt;CFArray>?

Returns the component registrations for a given audio unit extension.

func AudioUnitExtensionSetComponentList(CFString, CFArray?) -> OSStatus

Allows the implementor of an audio unit extension to dynamically modify the list of component registrations for the extension.

protocol AUAudioUnitFactory

An object that creates a version 3 audio unit.

