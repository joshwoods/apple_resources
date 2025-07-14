

- Audio Toolbox
-  AUAudioUnitPreset 

Class

# AUAudioUnitPreset

A class that describes an interface for custom parameter settings provided by the audio unit developer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class AUAudioUnitPreset
```

## Overview

These presets often produce a useful sound or starting point.

For more details on working with Audio Unit presets, see Audio Units - How to correctly save and restore Audio Unit presets. Note that the version 3 fullState property is bridged to the version 2 `kAudioUnitProperty_ClassInfo` API. Similarly, the version 3 fullStateForDocument property is bridged to the version 2 `kAudioUnitProperty_ClassInfoFromDocument` API.

## Topics

### Preset Properties

var name: String

The preset’s name.

var number: Int

The preset’s unique numeric identifier.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

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

class AUAudioUnitV2Bridge

A class that wraps a version 2 audio unit as version 3 audio unit.

func AudioUnitExtensionCopyComponentList(CFString) -> Unmanaged&lt;CFArray>?

Returns the component registrations for a given audio unit extension.

func AudioUnitExtensionSetComponentList(CFString, CFArray?) -> OSStatus

Allows the implementor of an audio unit extension to dynamically modify the list of component registrations for the extension.

protocol AUAudioUnitFactory

An object that creates a version 3 audio unit.

