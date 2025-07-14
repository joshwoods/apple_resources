

- AVFAudio
- AVAudioRecorder
-  init(url:format:) 

Initializer

# init(url:format:)

Creates an audio recorder with an audio format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    url: URL,
    format: AVAudioFormat
) throws
```

## Parameters 

`url`  

The file system location to record to.

`format`  

The audio format to use for the recording.

## Return Value

A new audio recorder, or nil if an error occurred.

## See Also

### Creating an audio recorder

init(url: URL, settings: [String : Any]) throws

Creates an audio recorder with settings.

