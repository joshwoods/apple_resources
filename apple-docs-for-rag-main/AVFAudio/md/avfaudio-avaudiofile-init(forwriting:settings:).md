

- AVFAudio
- AVAudioFile
-  init(forWriting:settings:) 

Initializer

# init(forWriting:settings:)

Opens a file for writing using the specified settings.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    forWriting fileURL: URL,
    settings: [String : Any]
) throws
```

## Parameters 

`fileURL`  

The path of the file to create for writing.

`settings`  

The format of the file to create.

## Return Value

A new `AVAudioFile` instance for writing.

## Discussion

This method infers the file type to create from the file extension of `fileURL`, and overwrites a file at the specified URL if a file exists.

The file opens for writing using the standard format AVAudioCommonFormat.pcmFormatFloat32. For more information about the `settings` parameter, see the settings property in the AVAudioRecorder class.

## See Also

### Related Documentation

var url: URL

The location of the audio file.

### Creating an Audio File

init(forReading: URL) throws

Opens a file for reading using the standard, deinterleaved floating point format.

init(forReading: URL, commonFormat: AVAudioCommonFormat, interleaved: Bool) throws

Opens a file for reading using the specified processing format.

init(forWriting: URL, settings: [String : Any], commonFormat: AVAudioCommonFormat, interleaved: Bool) throws

Opens a file for writing using a specified processing format and settings.

