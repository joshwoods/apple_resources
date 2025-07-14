

- Audio Toolbox
-  AudioUnitExtensionCopyComponentList(\_:) 

Function

# AudioUnitExtensionCopyComponentList(\_:)

Returns the component registrations for a given audio unit extension.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func AudioUnitExtensionCopyComponentList(_ extensionIdentifier: CFString) -> Unmanaged?
```

## Parameters 

`extensionIdentifier`  

The bundle identifier of the audio unit extension.

## Return Value

An array of component registrations.

## Discussion

This function returns an array of dictionaries (one dictionary for each registration component) in the same format as described in Audio Components.

Release this value when you’re done with it.

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

func AudioUnitExtensionSetComponentList(CFString, CFArray?) -> OSStatus

Allows the implementor of an audio unit extension to dynamically modify the list of component registrations for the extension.

protocol AUAudioUnitFactory

An object that creates a version 3 audio unit.

