

- Audio Toolbox
-  AUAudioUnitV2Bridge 

Class

# AUAudioUnitV2Bridge

A class that wraps a version 2 audio unit as version 3 audio unit.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class AUAudioUnitV2Bridge
```

## Overview

A version 3 audio unit may subclass the AUAudioUnitV2Bridge class. If so, the audio unit’s component description should refer to a registered component with a version 2 implementation by using a factory function. The bridge will instantiate the version 2 audio unit via the factory function and communicate with it using version 2 audio unit APIs.

Hosts should not access this class; it will be instantiated if needed when creating an audio unit.

## Topics

### Instance Properties

var audioUnit: AudioUnit

## Relationships

### Inherits From

- AUAudioUnit

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

class AUAudioUnitBus

A class that defines an input or output connection point on an audio unit.

class AUAudioUnitBusArray

A class that defines a container for an audio unit’s input or output busses.

class AUAudioUnitPreset

A class that describes an interface for custom parameter settings provided by the audio unit developer.

func AudioUnitExtensionCopyComponentList(CFString) -> Unmanaged&lt;CFArray>?

Returns the component registrations for a given audio unit extension.

func AudioUnitExtensionSetComponentList(CFString, CFArray?) -> OSStatus

Allows the implementor of an audio unit extension to dynamically modify the list of component registrations for the extension.

protocol AUAudioUnitFactory

An object that creates a version 3 audio unit.

