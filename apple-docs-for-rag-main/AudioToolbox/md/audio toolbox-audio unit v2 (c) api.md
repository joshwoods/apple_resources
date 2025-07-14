

- Audio Toolbox
-  Audio Unit v2 (C) API 

API Collection

# Audio Unit v2 (C) API

Configure an Audio Unit and prepare it to render audio.

## Topics

### Initializing the Audio Unit

func AudioUnitInitialize(AudioUnit) -> OSStatus

Initializes an audio unit

func AudioUnitUninitialize(AudioUnit) -> OSStatus

Uninitializes an audio unit.

func AudioUnitProcess(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

func AudioUnitProcessMultiple(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UInt32, UnsafeMutablePointer&lt;UnsafePointer&lt;AudioBufferList>>, UInt32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;AudioBufferList>>) -> OSStatus

func AudioUnitReset(AudioUnit, AudioUnitScope, AudioUnitElement) -> OSStatus

Resets an audio unit’s render state.

typealias AudioUnit

The data type for a plug-in component that provides audio processing or audio data generation.

### Starting and Stopping Output

func AudioOutputUnitStart(AudioUnit) -> OSStatus

Starts an I/O audio unit, which in turn starts the audio unit processing graph that it is connected to.

func AudioOutputUnitStop(AudioUnit) -> OSStatus

Stops an I/O audio unit, which in turn stops the audio unit processing graph that it is connected to.

typealias AudioOutputUnitStartProc

typealias AudioOutputUnitStopProc

### Rendering the Audio

func AudioUnitRender(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UInt32, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Initiates a rendering cycle for an audio unit.

func AudioUnitAddRenderNotify(AudioUnit, AURenderCallback, UnsafeMutableRawPointer?) -> OSStatus

Registers a callback to receive audio unit render notifications.

func AudioUnitRemoveRenderNotify(AudioUnit, AURenderCallback, UnsafeMutableRawPointer?) -> OSStatus

Unregisters a previously-registered render listener callback function.

typealias AURenderCallback

Called by the system when an audio unit requires input samples, or before and after a render operation.

struct AudioUnitRenderActionFlags

Flags for configuring audio unit rendering.

### Configuring Audio Unit Properties

func AudioUnitGetProperty(AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets the value of an audio unit property.

func AudioUnitSetProperty(AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeRawPointer?, UInt32) -> OSStatus

Sets the value of an audio unit property.

func AudioUnitGetPropertyInfo(AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about an audio unit property.

func AudioUnitAddPropertyListener(AudioUnit, AudioUnitPropertyID, AudioUnitPropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Registers a callback to receive audio unit property change notifications.

func AudioUnitRemovePropertyListenerWithUserData(AudioUnit, AudioUnitPropertyID, AudioUnitPropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Unregisters a previously-registered property listener callback function.

### Responding to Events

func AUEventListenerCreateWithDispatchQueue(UnsafeMutablePointer&lt;AUEventListenerRef?>, Float32, Float32, dispatch_queue_t, AUEventListenerBlock) -> OSStatus

func AUEventListenerCreate(AUEventListenerProc, UnsafeMutableRawPointer?, CFRunLoop?, CFString?, Float32, Float32, UnsafeMutablePointer&lt;AUEventListenerRef?>) -> OSStatus

func AUListenerDispose(AUParameterListenerRef) -> OSStatus

func AUEventListenerNotify(AUEventListenerRef?, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitEvent>) -> OSStatus

func AUEventListenerAddEventType(AUEventListenerRef, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitEvent>) -> OSStatus

func AUEventListenerRemoveEventType(AUEventListenerRef, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitEvent>) -> OSStatus

func AUListenerAddParameter(AUParameterListenerRef, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitParameter>) -> OSStatus

func AUListenerRemoveParameter(AUParameterListenerRef, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitParameter>) -> OSStatus

typealias AUEventListenerBlock

### Getting and Setting Parameters

func AudioUnitGetParameter(AudioUnit, AudioUnitParameterID, AudioUnitScope, AudioUnitElement, UnsafeMutablePointer&lt;AudioUnitParameterValue>) -> OSStatus

Gets the value of an audio unit parameter.

func AudioUnitScheduleParameters(AudioUnit, UnsafePointer&lt;AudioUnitParameterEvent>, UInt32) -> OSStatus

Schedules changes to the value of an audio unit parameter.

func AudioUnitSetParameter(AudioUnit, AudioUnitParameterID, AudioUnitScope, AudioUnitElement, AudioUnitParameterValue, UInt32) -> OSStatus

Sets the value of an audio unit parameter.

### Monitoring Parameter Changes

func AUListenerCreateWithDispatchQueue(UnsafeMutablePointer&lt;AUParameterListenerRef?>, Float32, dispatch_queue_t, AUParameterListenerBlock) -> OSStatus

func AUListenerCreate(AUParameterListenerProc, UnsafeMutableRawPointer, CFRunLoop?, CFString?, Float32, UnsafeMutablePointer&lt;AUParameterListenerRef?>) -> OSStatus

func AUParameterListenerNotify(AUParameterListenerRef?, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitParameter>) -> OSStatus

func AUParameterFormatValue(Float64, UnsafePointer&lt;AudioUnitParameter>, UnsafeMutablePointer&lt;CChar>, UInt32) -> UnsafeMutablePointer&lt;CChar>

func AUParameterSet(AUParameterListenerRef?, UnsafeMutableRawPointer?, UnsafePointer&lt;AudioUnitParameter>, AudioUnitParameterValue, UInt32) -> OSStatus

func AUParameterValueFromLinear(Float32, UnsafePointer&lt;AudioUnitParameter>) -> AudioUnitParameterValue

func AUParameterValueToLinear(AudioUnitParameterValue, UnsafePointer&lt;AudioUnitParameter>) -> Float32

typealias AUParameterListenerBlock

typealias AUParameterListenerProc

typealias AUParameterListenerRef

typealias AUImplementorDisplayNameWithLengthCallback

A block called to obtain a parameter node’s display name, possibly truncated to a desired length.

typealias AUImplementorStringFromValueCallback

A block called to convert a parameter value to a string representation.

typealias AUImplementorValueFromStringCallback

A block called to convert a string to a parameter value.

### Getting Information from the Host

typealias HostCallback_GetBeatAndTempo

When called by the system, provides beat and tempo information to an audio unit from a host application.

typealias HostCallback_GetMusicalTimeLocation

When called by the system, provides musical timing information to an audio unit from a host application.

typealias HostCallback_GetTransportState

When called by the system, provides audio transport state and timeline information to an audio unit from a host application.

typealias HostCallback_GetTransportState2

typealias AUInputSamplesInOutputCallback

Called by the system when an audio unit has provided a buffer of output samples.

typealias AUMIDIOutputCallback

When called by a host application, gets MIDI data from an audio unit.

### Getting the Configuration Information

var kAudioUnitConfigurationInfo_BusCountWritable: String

var kAudioUnitConfigurationInfo_ChannelConfigurations: String

var kAudioUnitConfigurationInfo_HasCustomView: String

var kAudioUnitConfigurationInfo_IconURL: String

var kAudioUnitConfigurationInfo_InitialInputs: String

var kAudioUnitConfigurationInfo_InitialOutputs: String

var kAudioUnitConfigurationInfo_SupportedChannelLayoutTags: String

### Configuring the Audio Unit UI

struct AudioUnitCocoaViewInfo

The name and number of custom Cocoa views for an audio unit.

func GetAudioUnitParameterDisplayType(AudioUnitParameterOptions) -> AudioUnitParameterOptions

func SetAudioUnitParameterDisplayType(AudioUnitParameterOptions, AudioUnitParameterOptions) -> AudioUnitParameterOptions

### Audio Unit Types

struct ScheduledAudioFileRegion

struct ScheduledAudioSlice

typealias ScheduledAudioFileRegionCompletionProc

typealias ScheduledAudioSliceCompletionProc

typealias MIDIChannelNumber

MIDI Channel, 0~15 (channels 1 through 16, respectively).

typealias AUAudioObjectID

typealias AUMIDICIProfileChangedBlock

typealias AUAudioChannelCount

A number of audio channels.

typealias AUAudioFrameCount

A number of audio sample frames.

typealias AUAudioUnitStatus

A result code returned from an audio unit’s render function.

typealias AUEventListenerProc

typealias AUEventListenerRef

typealias AUEventSampleTime

Expresses time as a sample count.

typealias AUImplementorValueObserver

A block called to notify the audio unit implementation of changes to a parameter value.

typealias AUImplementorValueProvider

A block called to fetch a parameter’s current value from the audio unit implementation.

typealias AUInputHandler

A block to notify the host of an I/O unit that an input is available.

typealias AUNodeConnection

typealias AUParameterAddress

A numeric identifier for an audio unit parameter.

typealias AUParameterAutomationObserver

typealias AUParameterObserver

A block called after the value of a parameter changes.

typealias AUParameterObserverToken

A token representing an installed parameter observer block.

typealias AUParameterRecordingObserver

A block called to record parameter changes as automation events.

typealias AURenderBlock

A block to render the audio unit.

typealias AURenderObserver

A block called when an audio unit renders audio.

typealias AURenderPullInputBlock

A block to supply audio input to a render block.

typealias AUScheduleParameterBlock

A block to schedule parameter changes.

typealias AUValue

A value of an audio unit parameter.

typealias AudioUnitAddPropertyListenerProc

typealias AudioUnitAddRenderNotifyProc

typealias AudioUnitComplexRenderProc

typealias AudioUnitElement

The data type for an audio unit element identifier.

typealias AudioUnitGetParameterProc

typealias AudioUnitGetPropertyInfoProc

typealias AudioUnitGetPropertyProc

typealias AudioUnitInitializeProc

typealias AudioUnitParameterID

The data type for an audio unit parameter identifier.

struct AudioUnitParameterNameInfo

A short version of the name for an audio unit parameter.

typealias AudioUnitParameterIDName

A type definition for a data type that defines the short version of the name for an audio unit parameter.

typealias AudioUnitParameterValue

The data type for an audio unit parameter value.

typealias AudioUnitProcessMultipleProc

typealias AudioUnitProcessProc

typealias AudioUnitPropertyID

The data type for audio unit property keys.

typealias AudioUnitPropertyListenerProc

Called by the system when the value of a specified audio unit property has changed.

typealias AudioUnitRemoteControlEventListener

typealias AudioUnitRemovePropertyListenerProc

typealias AudioUnitRemovePropertyListenerWithUserDataProc

typealias AudioUnitRemoveRenderNotifyProc

typealias AudioUnitRenderProc

typealias AudioUnitResetProc

typealias AudioUnitScheduleParametersProc

typealias AudioUnitScope

The data type for audio unit scope identifiers.

typealias AudioUnitSetParameterProc

typealias AudioUnitSetPropertyProc

typealias AudioUnitUninitializeProc

### Enumerations

Audio Unit Types

The defined types of audio processing plug-ins known as audio units.

Inter-App Audio Unit Types

Audio Unit Manufacturer Identifier

The Apple audio unit manufacturer code.

Audio Unit Output Subtypes

I/O Audio Unit Subtypes

Converter Audio Unit Subtypes

Audio data format converter audio unit subtypes for audio units provided by Apple.

Reserved Audio Unit Clump Identifier

Reserved for system use.

Offline Audio Unit Properties

Properties for audio units that perform offline processing—that is, processing in a nonplayback, nonrealtime mode.

MIDI Audio Unit Parameters

Parameters for instrument units.

General Audio Unit Function Selectors

General audio unit component selectors that correspond to functions in the audio unit API.

Generator Audio Unit Subtypes

Audio units that serve as sound sources.

Input/Output Audio Unit Subtypes

Input/output audio unit subtypes for audio units provided by Apple.

Audio Unit Panner Subtypes

Audio Unit Player Subtypes

Audio Unit Pitch Subtypes

enum AudioUnitEventType

struct AudioUnitParameterOptions

Value options for audio unit parameters.

enum AudioUnitParameterUnit

The unit-of-measure for an audio unit parameter.

enum AudioUnitRemoteControlEvent

Audio Unit Sample Rate Converter Complexity

Quality levels for the audio sample-rate conversion algorithm.

Audio Unit Scopes

Programmatic roles and contexts for audio unit properties.

Audio Unit SRC Algorithms

Audio Unit Full Name Parameter

Audio Unit Parameter Flags

Audio Unit Filter Parameters

Audio Unit Generic Properties

Audio Unit Parameter Flags

Audio Unit Scheduled Sound Player Properties

Audio Unit Offline Preflight Flags

Audio Unit Migration Properties

Audio Unit File Player Properties

Audio Unit Parameter Listener

Audio Unit Errors

enum AUAudioUnitBusType

AUEventSampleTime

Expresses time as a sample count.

struct AUHostTransportStateFlags

enum AUParameterAutomationEventType

enum AUParameterEventType

Audio unit parameter event types.

enum AURenderEventType

struct AUScheduledAudioSliceFlags

struct AUParameterMIDIMappingFlags

## See Also

### Audio Units

Generating spatial audio from a multichannel audio stream

Convert 8-channel audio to 2-channel spatial audio by using a spatial mixer audio unit.

Audio Unit v3 Plug-Ins

Deliver custom audio effects, instruments, and other audio behaviors using an Audio Unit v3 app extension.

Audio Components

Find, load, and configure audio components, such as Audio Units and audio codecs.

Audio Unit Properties

Obtain information about the built-in mixers, equalizers, filters, effects, and other Audio Unit app extensions.

Audio Unit Voice I/O

Configure system voice processing and respond to speech events.

