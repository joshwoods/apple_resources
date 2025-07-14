

- Audio Toolbox
- Audio Unit Properties
-  General Audio Unit Properties 

API Collection

# General Audio Unit Properties

Properties that apply to any audio unit.

## Overview

The integer range for the set of generic audio unit property identifiers is 0 through 999.

## Topics

### Properties

var kAudioUnitProperty_ElementCount: AudioUnitPropertyID

A read/write `UInt32` value valid on any audio unit scope. The global audio unit scope always has an element count of 1.

var kAudioUnitProperty_SupportedNumChannels: AudioUnitPropertyID

A read-only array of channel information structures valid on the audio unit global scope.

var kAudioUnitProperty_AudioChannelLayout: AudioUnitPropertyID

A read/write `AudioChannelLayout` data structure valid on the audio unit input and output scopes.

var kAudioUnitProperty_AudioUnitMIDIProtocol: AudioUnitPropertyID

var kAudioUnitProperty_AUHostIdentifier: AudioUnitPropertyID

var kAudioUnitProperty_BypassEffect: AudioUnitPropertyID

A read/write `UInt32` value, representing a Boolean value, valid on the audio unit global scope.

var kAudioUnitProperty_ClassInfo: AudioUnitPropertyID

Describes the state of an audio unit.

var kAudioUnitProperty_ClassInfoFromDocument: AudioUnitPropertyID

A read/write CFDictionary object, valid on the audio unit global scope.

var kAudioUnitProperty_CocoaUI: AudioUnitPropertyID

A read-only `AudioUnitCocoaViewInfo` data structure valid on the audio unit global scope.

var kAudioUnitProperty_ContextName: AudioUnitPropertyID

var kAudioUnitProperty_CPULoad: AudioUnitPropertyID

A read-only `Float64` value valid on the audio unit global scope.

var kAudioUnitProperty_DependentParameters: AudioUnitPropertyID

var kAudioUnitProperty_ElementName: AudioUnitPropertyID

The name of the specified element.

var kAudioUnitProperty_FactoryPresets: AudioUnitPropertyID

So-called *factory presets* (as opposed to user-configured presets) are ones supplied with an audio unit by the manufacturer. You choose the active preset by setting the `kAudioUnitProperty_PresentPreset` property.

var kAudioUnitProperty_FastDispatch: AudioUnitPropertyID

A read-only `void *` value valid on the audio unit global scope.

var kAudioUnitProperty_FrequencyResponse: AudioUnitPropertyID

var kAudioUnitProperty_GetUIComponentList: AudioUnitPropertyID

var kAudioUnitProperty_HostCallbacks: AudioUnitPropertyID

var kAudioUnitProperty_HostMIDIProtocol: AudioUnitPropertyID

var kAudioUnitProperty_IconLocation: AudioUnitPropertyID

var kAudioUnitProperty_InPlaceProcessing: AudioUnitPropertyID

A read/write `UInt32` value, representing a Boolean value, valid on the audio unit global scope.

var kAudioUnitProperty_InputSamplesInOutput: AudioUnitPropertyID

A read/write AUInputSamplesInOutputCallbackStruct struct, valid on the audio unit global scope.

var kAudioUnitProperty_LastRenderError: AudioUnitPropertyID

A read-only `OSStatus` value valid on the audio unit global scope.

var kAudioUnitProperty_LastRenderSampleTime: AudioUnitPropertyID

var kAudioUnitProperty_Latency: AudioUnitPropertyID

A read-only `Float64` value valid on the audio unit global scope.

var kAudioUnitProperty_LoadedOutOfProcess: AudioUnitPropertyID

var kAudioUnitProperty_MakeConnection: AudioUnitPropertyID

A write-only AudioUnitConnection data structure valid on the audio unit input scope.

var kAudioUnitProperty_MIDIOutputBufferSizeHint: AudioUnitPropertyID

var kAudioUnitProperty_MIDIOutputCallback: AudioUnitPropertyID

A write-only AUMIDIOutputCallbackStruct struct, valid on the audio unit global scope.

var kAudioUnitProperty_MIDIOutputCallbackInfo: AudioUnitPropertyID

A read-only CFArray object valid on the audio unit global scope.

var kAudioUnitProperty_MIDIOutputEventListCallback: AudioUnitPropertyID

var kAudioUnitProperty_MaximumFramesPerSlice: AudioUnitPropertyID

Specifies the maximum number of sample frames an audio unit is prepared to supply on one invocation of its AudioUnitRender(_:_:_:_:_:_:) function.

var kAudioUnitProperty_NickName: AudioUnitPropertyID

var kAudioUnitProperty_OfflineRender: AudioUnitPropertyID

var kAudioUnitProperty_ParameterClumpName: AudioUnitPropertyID

A read-only `AudioUnitParameterNameInfo` struct, valid on any audio unit scope.

var kAudioUnitProperty_ParameterHistoryInfo: AudioUnitPropertyID

For parameters that have the flag_PlotHistory flag set, getting this property fills out the AudioUnitParameterHistoryInfo struct containing the recommended update rate and history duration.

var kAudioUnitProperty_ParameterIDName: AudioUnitPropertyID

A shortened version of an audio unit parameter name, suitable for compact display situations.

var kAudioUnitProperty_ParameterInfo: AudioUnitPropertyID

var kAudioUnitProperty_ParameterList: AudioUnitPropertyID

A list of read-only parameter ID values valid on any audio unit scope.

var kAudioUnitProperty_ParameterStringFromValue: AudioUnitPropertyID

A read-only AudioUnitParameterStringFromValue struct, valid on any audio unit scope.

var kAudioUnitProperty_ParameterValueFromString: AudioUnitPropertyID

var kAudioUnitProperty_ParameterValueStrings: AudioUnitPropertyID

An array of names for a named, indexed audio unit parameter. An indexed parameter is one whose unit type is AudioUnitParameterUnit.indexed. The array’s strings can be used to build a menu for the parameter.

var kAudioUnitProperty_ParametersForOverview: AudioUnitPropertyID

var kAudioUnitProperty_PresentPreset: AudioUnitPropertyID

The active factory preset for an audio unit.

var kAudioUnitProperty_PresentationLatency: AudioUnitPropertyID

var kAudioUnitProperty_RenderQuality: AudioUnitPropertyID

A read/write `UInt32` value valid on the audio unit global scope.

var kAudioUnitProperty_RequestViewController: AudioUnitPropertyID

var kAudioUnitProperty_SampleRate: AudioUnitPropertyID

var kAudioUnitProperty_SetExternalBuffer: AudioUnitPropertyID

var kAudioUnitProperty_SetRenderCallback: AudioUnitPropertyID

var kAudioUnitProperty_StreamFormat: AudioUnitPropertyID

var kAudioUnitProperty_ShouldAllocateBuffer: AudioUnitPropertyID

A read/write `UInt32` value valid on the audio unit input and output scopes, settable individually on each element.

var kAudioUnitProperty_SupportedChannelLayoutTags: AudioUnitPropertyID

A read-only array on `AudioChannelLayoutTag` structures, valid on the audio unit input and output scopes.

var kAudioUnitProperty_SupportsMPE: AudioUnitPropertyID

var kAudioUnitProperty_TailTime: AudioUnitPropertyID

A read-only `Float64` value valid on the audio unit global scope.

## See Also

### General

Other Plug-In Formats

RenderQuality

Render quality settings for audio units.

struct HostCallbackInfo

The time- and transport-related callback functions for an audio unit.

