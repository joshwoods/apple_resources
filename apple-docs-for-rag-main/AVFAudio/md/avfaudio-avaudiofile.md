

- AVFAudio
-  AVAudioFile 

Class

# AVAudioFile

An object that represents an audio file that the system can open for reading or writing.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioFile
```

## Overview

Regardless of the file format, you read and write using AVAudioPCMBuffer objects. These objects contain samples as AVAudioCommonFormat that the framework refers to as the file’s processing format. You convert to and from using the file’s actual format.

Reads and writes are always sequential. Random access is possible by setting the framePosition property.

## Topics

### Creating an Audio File

init(forReading: URL) throws

Opens a file for reading using the standard, deinterleaved floating point format.

init(forReading: URL, commonFormat: AVAudioCommonFormat, interleaved: Bool) throws

Opens a file for reading using the specified processing format.

init(forWriting: URL, settings: [String : Any]) throws

Opens a file for writing using the specified settings.

init(forWriting: URL, settings: [String : Any], commonFormat: AVAudioCommonFormat, interleaved: Bool) throws

Opens a file for writing using a specified processing format and settings.

### Reading and Writing the Audio Buffer

func read(into: AVAudioPCMBuffer) throws

Reads an entire audio buffer.

func read(into: AVAudioPCMBuffer, frameCount: AVAudioFrameCount) throws

Reads a portion of an audio buffer using the number of frames you specify.

func write(from: AVAudioPCMBuffer) throws

Writes an audio buffer sequentially.

func close()

Closes the audio file.

### Getting Audio File Properties

var url: URL

The location of the audio file.

var fileFormat: AVAudioFormat

The on-disk format of the file.

var processingFormat: AVAudioFormat

The processing format of the file.

var length: AVAudioFramePosition

The number of sample frames in the file.

typealias AVAudioFramePosition

A position in an audio file or stream.

var framePosition: AVAudioFramePosition

The position in the file where the next read or write operation occurs.

typealias AVAudioFrameCount

A number of audio sample frames.

let AVAudioFileTypeKey: String

A string that indicates the audio file type.

var isOpen: Bool

A Boolean value that indicates whether the file is open.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Supporting data types

class AVAudioBuffer

An object that represents a buffer of audio data with a format.

class AVAudioTime

An object you use to represent a moment in time.

Audio settings

Configure audio processing settings using standard key and value constants.

