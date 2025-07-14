

- Audio Toolbox
-  Audio Toolbox Debugging 

API Collection

# Audio Toolbox Debugging

Obtain the internal state of Core Audio objects during the development and debugging of your code.

## Overview

The `AudioToolbox.h` header file provides auxiliary functions for obtaining the internal state of a Core Audio object. Use these functions during development and debugging.

## Topics

### Audio Toolbox Debugging Functions

func CAShow(UnsafeMutableRawPointer)

Prints the internal state of an object to `stdio`.

func CAShowFile(UnsafeMutableRawPointer, UnsafeMutablePointer&lt;FILE>)

Prints the internal state of an object to a file.

### Instrument Functions

func CopyNameFromSoundBank(CFURL, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Copies the name of a sound bank from a sound bank file at a specified URL.

func CopyInstrumentInfoFromSoundBank(CFURL, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>) -> OSStatus

var kInstrumentInfoKey_LSB: String

var kInstrumentInfoKey_MSB: String

var kInstrumentInfoKey_Name: String

var kInstrumentInfoKey_Program: String

### Constants

var AUDIO_TOOLBOX_VERSION: Int32

## See Also

### Utilities

Analyzing audio performance with Instruments

Ensure a smooth and immersive audio experience in your apps using Audio System Trace.

Audio Converter Services

Convert between linear PCM audio formats, and between linear PCM and compressed formats.

Audio Session Support

Describe the properties that you associate with audio sessions and audio routes.

Workgroup Management

Coordinate the activity of custom real-time audio threads with those of the system and other processes.

Audio Codec

Translate audio data from one format to another.

Clock Utilities

Manage time-related information associated with audio playback.

