

- AVFAudio
- AVAudioFile
-  init(forReading:) 

Initializer

# init(forReading:)

Opens a file for reading using the standard, deinterleaved floating point format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(forReading fileURL: URL) throws
```

## Parameters 

`fileURL`  

The file to read.

## Return Value

A new `AVAudioFile` instance you use for reading.

## See Also

### Creating an Audio File

init(forReading: URL, commonFormat: AVAudioCommonFormat, interleaved: Bool) throws

Opens a file for reading using the specified processing format.

init(forWriting: URL, settings: [String : Any]) throws

Opens a file for writing using the specified settings.

init(forWriting: URL, settings: [String : Any], commonFormat: AVAudioCommonFormat, interleaved: Bool) throws

Opens a file for writing using a specified processing format and settings.

