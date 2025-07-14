

- Audio Toolbox
-  Audio Unit v3 Plug-Ins 

API Collection

# Audio Unit v3 Plug-Ins

Deliver custom audio effects, instruments, and other audio behaviors using an Audio Unit v3 app extension.

## Topics

### Host App

Migrating Your Audio Unit Host to the AUv3 API

Update your Audio Unit (AU) host app to take advantage of the new features and capabilities of AUv3.

Hosting Audio Unit Extensions Using the AUv2 API

Update your existing Audio Unit v2 host app to load and use Audio Unit extensions.

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

protocol AUAudioUnitFactory

An object that creates a version 3 audio unit.

### Parameters

class AUParameter

An object that represents a single audio unit parameter.

class AUParameterGroup

A parameter group object represents a group of related audio unit parameters.

class AUParameterNode

An object that represents a node in an audio unit’s parameter tree.

class AUParameterTree

An object that represents a top-level group node that contains all of an audio unit’s parameters.

## See Also

### Audio Units

Generating spatial audio from a multichannel audio stream

Convert 8-channel audio to 2-channel spatial audio by using a spatial mixer audio unit.

Audio Components

Find, load, and configure audio components, such as Audio Units and audio codecs.

Audio Unit v2 (C) API

Configure an Audio Unit and prepare it to render audio.

Audio Unit Properties

Obtain information about the built-in mixers, equalizers, filters, effects, and other Audio Unit app extensions.

Audio Unit Voice I/O

Configure system voice processing and respond to speech events.

