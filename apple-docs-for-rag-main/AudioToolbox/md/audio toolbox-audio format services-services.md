

- Audio Toolbox
-  Audio Format Services 

API Collection

# Audio Format Services

Access information about audio formats and codecs.

## Overview

This document describes Audio Format Services, a C interface for obtaining information about audio formats and codecs.

## Topics

### Audio Format Services Functions

func AudioFormatGetProperty(AudioFormatPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutableRawPointer?) -> OSStatus

Gets the value of an audio format property.

func AudioFormatGetPropertyInfo(AudioFormatPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets information about an audio format property.

### Data Types

struct AudioBalanceFade

Describes audio left/right balance and front/back fade values.

struct AudioFormatInfo

A structure that specifies an audio format.

struct AudioFormatListItem

struct AudioPanningInfo

Audio panning information.

struct ExtendedAudioFormatInfo

A specifier for the kAudioFormatProperty_FormatList property, including the codec to use.

typealias AudioFormatPropertyID

A type for four-char codes for audio format property identifiers.

### Constants

enum AudioBalanceFadeType

Identifiers for audio balance fade types.

Audio Format Property Identifiers

Constants for use with the AudioFormatGetPropertyInfo(_:_:_:_:) and AudioFormatGetProperty(_:_:_:_:_:) functions.

Audio Codec Component Constants

Audio codec component types.

Audio Codec Manufacturer and Implementation Types

Identifiers for audio codec manufacturers and implementation types.

enum AudioPanningMode

Identifiers for audio panning algorithms.

### Result Codes

This table lists the result codes defined for Audio Format Services.

Audio Format Error Codes

var kAudioFormatUnspecifiedError: OSStatus

An unspecified error.

var kAudioFormatUnsupportedPropertyError: OSStatus

The specified property is not supported.

var kAudioFormatBadPropertySizeError: OSStatus

var kAudioFormatBadSpecifierSizeError: OSStatus

var kAudioFormatUnsupportedDataFormatError: OSStatus

The playback data format is unsupported (declared in `AudioFormat.h`).

var kAudioFormatUnknownFormatError: OSStatus

The specified data format is not a known format.

## See Also

### Audio Files and Formats

Audio File Services

Read or write a variety of audio data to or from disk or a memory buffer.

Extended Audio File Services

Read and write compressed files and linear PCM audio files using a simplified interface.

Audio File Stream Services

Parse streamed audio files as the data arrives on the user’s computer.

Audio File Components

Get information about audio file formats, and about files containing audio data.

Core Audio File Format

Parse the structure of Core Audio files.

