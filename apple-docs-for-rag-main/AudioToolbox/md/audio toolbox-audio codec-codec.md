

- Audio Toolbox
-  Audio Codec 

API Collection

# Audio Codec

Translate audio data from one format to another.

## Topics

### Initializing an Audio Codec

func AudioCodecInitialize(AudioCodec, UnsafePointer&lt;AudioStreamBasicDescription>?, UnsafePointer&lt;AudioStreamBasicDescription>?, UnsafeRawPointer?, UInt32) -> OSStatus

Sets up the specified codec to perform a data format translation.

func AudioCodecReset(AudioCodec) -> OSStatus

Flushes all the audio data in the codec and clears the input buffer.

func AudioCodecUninitialize(AudioCodec) -> OSStatus

Moves the codec from the initialized state back to the uninitialized state.

### Configuring Buffers

func AudioCodecAppendInputBufferList(AudioCodec, UnsafePointer&lt;AudioBufferList>, UnsafeMutablePointer&lt;UInt32>, UnsafePointer&lt;AudioStreamPacketDescription>?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioCodecProduceOutputBufferList(AudioCodec, UnsafeMutablePointer&lt;AudioBufferList>, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

### Accessing the Data

func AudioCodecAppendInputData(AudioCodec, UnsafeRawPointer, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;UInt32>, UnsafePointer&lt;AudioStreamPacketDescription>?) -> OSStatus

Appends audio data to the codec’s input buffer.

func AudioCodecProduceOutputPackets(AudioCodec, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Retrieves output data from a codec.

### Accessing Codec Properties

func AudioCodecGetProperty(AudioCodec, AudioCodecPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Retrieves the value of a codec property.

func AudioCodecGetPropertyInfo(AudioCodec, AudioCodecPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Retrieves information about a codec property.

func AudioCodecSetProperty(AudioCodec, AudioCodecPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value of a codec property.

### Codec Types

struct AudioCodecMagicCookieInfo

A structure holding magic cookie information needed by some codecs.

struct AudioCodecPrimeInfo

A structure specifying the number of leading and trailing empty frames to be inserted.

typealias AudioCodec

An instance of a Component Manager component.

typealias AudioCodecAppendInputBufferListProc

typealias AudioCodecAppendInputDataProc

typealias AudioCodecGetPropertyInfoProc

typealias AudioCodecGetPropertyProc

typealias AudioCodecInitializeProc

typealias AudioCodecProduceOutputBufferListProc

typealias AudioCodecProduceOutputPacketsProc

typealias AudioCodecPropertyID

An integer identifying an audio codec property.

typealias AudioCodecResetProc

typealias AudioCodecSetPropertyProc

typealias AudioCodecUninitializeProc

### Audio Settings

struct AudioSettingsFlags

var kAudioSettings_AvailableValues: String

var kAudioSettings_CurrentValue: String

var kAudioSettings_Hint: String

var kAudioSettings_LimitedValues: String

var kAudioSettings_Parameters: String

var kAudioSettings_SettingKey: String

var kAudioSettings_SettingName: String

var kAudioSettings_Summary: String

var kAudioSettings_TopLevelKey: String

var kAudioSettings_Unit: String

var kAudioSettings_ValueType: String

var kAudioSettings_Version: String

### Enumerations

Output Status Constants

Status values returned from the AudioCodecProduceOutputPackets(_:_:_:_:_:_:) function.

Program Target Levels

Dynamic Range Control Modes

Bit Rate Control Mode Constants

Bit rate control modes to be used with `kAudioCodecPropertyBitRateControlMode`.

Global Codec Properties

These read-only properties disclose the capabilities of the codec and remain the same for all instances of the codec.

Instance Codec Properties

Properties that can be set or read on an instance of the audio codec.

Audio Codec Priming Method Constants

Values used with `kAudioCodecPropertyPrimeMethod`.

Audio Codec Quality Constants

Sound quality settings to be used with the property `kAudioCodecPropertyQualitySetting`.

Audio Codec Routine Selectors

Selectors used by the Component Manager to call routines implemented by the codec and exposed to developers through the Audio Codec Services API. These selectors are for use by codec developers; if you are calling Audio Codec Services functions, you don’t need to use these constants.

Audio Codec Delays

Audio Codec Delay Modes

Audio Codec Properties

Audio Codec Errors

## See Also

### Utilities

Analyzing audio performance with Instruments

Ensure a smooth and immersive audio experience in your apps using Audio System Trace.

Audio Converter Services

Convert between linear PCM audio formats, and between linear PCM and compressed formats.

Audio Session Support

Describe the properties that you associate with audio sessions and audio routes.

Audio Toolbox Debugging

Obtain the internal state of Core Audio objects during the development and debugging of your code.

Workgroup Management

Coordinate the activity of custom real-time audio threads with those of the system and other processes.

Clock Utilities

Manage time-related information associated with audio playback.

