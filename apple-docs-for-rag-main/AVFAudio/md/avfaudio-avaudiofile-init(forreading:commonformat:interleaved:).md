

- AVFAudio
- AVAudioFile
-  init(forReading:commonFormat:interleaved:) 

Initializer

# init(forReading:commonFormat:interleaved:)

Opens a file for reading using the specified processing format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    forReading fileURL: URL,
    commonFormat format: AVAudioCommonFormat,
    interleaved: Bool
) throws
```

## Parameters 

`fileURL`  

The file to read.

`format`  

The processing format to use when reading from the file.

`interleaved`  

The Boolean value that indicates whether to use an interleaved processing format.

## Return Value

A new `AVAudioFile` instance you use for reading.

## Discussion

The processing format refers to the buffers it reads from the file. The system reads the content and converts from the file format to the processing format. The processing format must be at the same sample rate as the actual file contents, and must be linear PCM. The interleaved parameter determines whether the processing buffer is in an interleaved float format.

## See Also

### Creating an Audio File

init(forReading: URL) throws

Opens a file for reading using the standard, deinterleaved floating point format.

init(forWriting: URL, settings: [String : Any]) throws

Opens a file for writing using the specified settings.

init(forWriting: URL, settings: [String : Any], commonFormat: AVAudioCommonFormat, interleaved: Bool) throws

Opens a file for writing using a specified processing format and settings.

