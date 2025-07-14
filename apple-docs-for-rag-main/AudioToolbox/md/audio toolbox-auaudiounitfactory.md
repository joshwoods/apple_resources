

- Audio Toolbox
-  AUAudioUnitFactory 

Protocol

# AUAudioUnitFactory

An object that creates a version 3 audio unit.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
protocol AUAudioUnitFactory : NSExtensionRequestHandling
```

## Overview

In most cases, if your audio unit specifies parameters to configure its behavior, it should provide a custom user interface to control those parameters. You create this user interface by subclassing the AUViewController class and implementing this protocol on your subclass.

If your audio unit doesn’t provide a custom user interface, subclass the NSObject class instead. In this case, the hosting app must create a generic user interface for your audio unit.

## Topics

### Required Methods

func createAudioUnit(with: AudioComponentDescription) throws -> AUAudioUnit

Creates an instance of an extension’s audio unit.

**Required**

## Relationships

### Inherits From

- NSExtensionRequestHandling
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

class AUAudioUnitV2Bridge

A class that wraps a version 2 audio unit as version 3 audio unit.

func AudioUnitExtensionCopyComponentList(CFString) -> Unmanaged&lt;CFArray>?

Returns the component registrations for a given audio unit extension.

func AudioUnitExtensionSetComponentList(CFString, CFArray?) -> OSStatus

Allows the implementor of an audio unit extension to dynamically modify the list of component registrations for the extension.

