

- Audio Toolbox
-  Extended Audio File Services 

API Collection

# Extended Audio File Services

Read and write compressed files and linear PCM audio files using a simplified interface.

## Overview

Extended Audio File Services provides simplified audio file access, combining features of Audio File Services and Audio Converter Services. It provides a unified interface for reading and writing compressed as well as linear PCM audio files.

## Topics

### Managing Extended Audio File Objects

func ExtAudioFileCreateWithURL(CFURL, AudioFileTypeID, UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioChannelLayout>?, UInt32, UnsafeMutablePointer&lt;ExtAudioFileRef?>) -> OSStatus

Creates a new audio file and associates it with a new extended audio file object.

func ExtAudioFileDispose(ExtAudioFileRef) -> OSStatus

Disposes of an extended audio file object and closes the associated file.

func ExtAudioFileOpenURL(CFURL, UnsafeMutablePointer&lt;ExtAudioFileRef?>) -> OSStatus

Opens an existing audio file for reading, and associates it with a new extended audio file object.

func ExtAudioFileWrapAudioFileID(AudioFileID, Bool, UnsafeMutablePointer&lt;ExtAudioFileRef?>) -> OSStatus

Wraps an audio file object in an extended audio file object.

### Configuring Properties for Extended Audio File Objects

func ExtAudioFileGetProperty(ExtAudioFileRef, ExtAudioFilePropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Gets a property value from an extended audio file object.

func ExtAudioFileGetPropertyInfo(ExtAudioFileRef, ExtAudioFilePropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about an extended audio file object property.

func ExtAudioFileSetProperty(ExtAudioFileRef, ExtAudioFilePropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets a property value for an extended audio file object.

### Reading and Writing Audio Data

func ExtAudioFileRead(ExtAudioFileRef, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Performs a synchronous, sequential read operation on an audio file.

func ExtAudioFileSeek(ExtAudioFileRef, Int64) -> OSStatus

Seeks to a specified frame in a file.

func ExtAudioFileTell(ExtAudioFileRef, UnsafeMutablePointer&lt;Int64>) -> OSStatus

Gets an audio file’s read/write position.

func ExtAudioFileWrite(ExtAudioFileRef, UInt32, UnsafePointer&lt;AudioBufferList>) -> OSStatus

Performs a synchronous, sequential write operation on an audio file.

func ExtAudioFileWriteAsync(ExtAudioFileRef, UInt32, UnsafePointer&lt;AudioBufferList>?) -> OSStatus

Perform an asynchronous, sequential write operation on an audio file.

### Data Types

typealias ExtAudioFilePacketTableInfoOverride

typealias ExtAudioFileRef

An opaque structure representing an extended audio file object.

typealias ExtAudioFilePropertyID

An audio file object property identifier.

### Constants

Extended Audio FIle Errors

Codec Unavailable Errors

Property Identifiers for Extended Audio File Objects

Extended Audio File Packet Overrides

### Result Codes

This table lists result codes defined for Extended Audio File Services.

var kExtAudioFileError_CodecUnavailableInputConsumed: OSStatus

The ExtAudioFileWrite(_:_:_:) function was interrupted and the last buffer that you provided was successfully written to disk.

var kExtAudioFileError_CodecUnavailableInputNotConsumed: OSStatus

The ExtAudioFileWrite(_:_:_:) function was interrupted and the last buffer that you provided was *not* successfully written to disk.

var kExtAudioFileError_InvalidProperty: OSStatus

var kExtAudioFileError_InvalidPropertySize: OSStatus

var kExtAudioFileError_NonPCMClientFormat: OSStatus

var kExtAudioFileError_InvalidChannelMap: OSStatus

The number of channels does not match the specified format.

var kExtAudioFileError_InvalidOperationOrder: OSStatus

var kExtAudioFileError_InvalidDataFormat: OSStatus

var kExtAudioFileError_MaxPacketSizeUnknown: OSStatus

var kExtAudioFileError_InvalidSeek: OSStatus

An attempt to write, or an offset, is out of bounds.

var kExtAudioFileError_AsyncWriteTooLarge: OSStatus

var kExtAudioFileError_AsyncWriteBufferOverflow: OSStatus

An asynchronous write operation could not be completed in time.

## See Also

### Audio Files and Formats

Audio Format Services

Access information about audio formats and codecs.

Audio File Services

Read or write a variety of audio data to or from disk or a memory buffer.

Audio File Stream Services

Parse streamed audio files as the data arrives on the user’s computer.

Audio File Components

Get information about audio file formats, and about files containing audio data.

Core Audio File Format

Parse the structure of Core Audio files.

