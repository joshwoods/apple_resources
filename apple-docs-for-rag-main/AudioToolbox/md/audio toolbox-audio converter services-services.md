

- Audio Toolbox
-  Audio Converter Services 

API Collection

# Audio Converter Services

Convert between linear PCM audio formats, and between linear PCM and compressed formats.

## Overview

Audio converter objects convert between various linear PCM audio formats. They can also convert between linear PCM and compressed formats. Supported transformations include the following:

- PCM bit depth

- PCM sample rate

- PCM floating point to and from PCM integer

- PCM interleaved to and from PCM deinterleaved

- PCM to and from compressed formats

A single audio converter may perform more than one of the listed transformations.

## Topics

### Managing Audio Converter Objects

func AudioConverterNew(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

Creates a new audio converter object based on specified audio formats.

func AudioConverterNewSpecific(UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, UnsafePointer&lt;AudioClassDescription>, UnsafeMutablePointer&lt;AudioConverterRef?>) -> OSStatus

Creates a new audio converter object using a specified codec.

func AudioConverterReset(AudioConverterRef) -> OSStatus

Resets an audio converter object, clearing and flushing its buffers.

func AudioConverterDispose(AudioConverterRef) -> OSStatus

Disposes of an audio converter object.

### Configuring Audio Converter Properties

func AudioConverterGetProperty(AudioConverterRef, AudioConverterPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Gets an audio converter property value.

func AudioConverterGetPropertyInfo(AudioConverterRef, AudioConverterPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about an audio converter property.

func AudioConverterSetProperty(AudioConverterRef, AudioConverterPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value of an audio converter object property.

### Performing Conversions

Encoding and decoding audio

Convert audio formats to efficiently manage data and quality.

func AudioConverterConvertBuffer(AudioConverterRef, UInt32, UnsafeRawPointer, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Converts audio data from one linear PCM format to another.

func AudioConverterFillComplexBuffer(AudioConverterRef, AudioConverterComplexInputDataProc, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioBufferList>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?) -> OSStatus

Converts audio data supplied by a callback function, supporting non-interleaved and packetized formats.

func AudioConverterConvertComplexBuffer(AudioConverterRef, UInt32, UnsafePointer&lt;AudioBufferList>, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Converts audio data from one linear PCM format to another, where both use the same sample rate.

### Callbacks

typealias AudioConverterComplexInputDataProc

Supplies input data to the AudioConverterFillComplexBuffer(_:_:_:_:_:_:) function.

typealias AudioConverterInputDataProc

Deprecated. Use AudioConverterFillComplexBuffer(_:_:_:_:_:_:) instead.

### Data Types

struct AudioConverterPrimeInfo

Specifies priming information for an audio converter.

typealias AudioConverterRef

A reference to an audio converter object.

typealias AudioConverterPropertyID

An audio converter property identifier.

### Constants

Audio Converter Properties

Audio converter properties, used with the AudioConverterGetPropertyInfo(_:_:_:_:), AudioConverterGetProperty(_:_:_:_:), and AudioConverterSetProperty(_:_:_:_:) functions.

Converter Priming Constants

Constants used with the kAudioConverterPrimeMethod property.

Sample Rate Conversion Quality Identifiers

Specifiers for sample rate conversion quality, used for the kAudioConverterSampleRateConverterQuality property.

Sample Rate Conversion Complexity Identifiers

Specifiers for the sample rate conversion algorithm, used for the kAudioConverterSampleRateConverterComplexity property.

### Enumerations

Converter Audio Unit Properties

Properties for the Apple AUConverter audio unit.

Converter Audio Unit Subtypes

Audio data format converter audio unit subtypes for audio units provided by Apple.

Audio Converter Dithering Algorithms

Audio Converter Properties (macOS)

Audio Converter Errors

### Result Codes

This table lists result codes defined for Audio Converter Services.

var kAudioConverterErr_FormatNotSupported: OSStatus

var kAudioConverterErr_OperationNotSupported: OSStatus

var kAudioConverterErr_PropertyNotSupported: OSStatus

var kAudioConverterErr_InvalidInputSize: OSStatus

var kAudioConverterErr_InvalidOutputSize: OSStatus

The byte size is not an integer multiple of the frame size.

var kAudioConverterErr_UnspecifiedError: OSStatus

var kAudioConverterErr_BadPropertySizeError: OSStatus

var kAudioConverterErr_RequiresPacketDescriptionsError: OSStatus

var kAudioConverterErr_InputSampleRateOutOfRange: OSStatus

var kAudioConverterErr_OutputSampleRateOutOfRange: OSStatus

var kAudioConverterErr_HardwareInUse: OSStatus

Returned from the AudioConverterFillComplexBuffer(_:_:_:_:_:_:) function if the underlying hardware codec has become unavailable, probably due to an audio interruption.

var kAudioConverterErr_NoHardwarePermission: OSStatus

Returned from the AudioConverterNew(_:_:_:) function if the new converter would use a hardware codec which the application does not have permission to use.

## See Also

### Utilities

Analyzing audio performance with Instruments

Ensure a smooth and immersive audio experience in your apps using Audio System Trace.

Audio Session Support

Describe the properties that you associate with audio sessions and audio routes.

Audio Toolbox Debugging

Obtain the internal state of Core Audio objects during the development and debugging of your code.

Workgroup Management

Coordinate the activity of custom real-time audio threads with those of the system and other processes.

Audio Codec

Translate audio data from one format to another.

Clock Utilities

Manage time-related information associated with audio playback.

