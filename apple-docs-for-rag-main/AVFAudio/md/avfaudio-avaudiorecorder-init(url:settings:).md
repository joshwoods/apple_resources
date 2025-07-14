

- AVFAudio
- AVAudioRecorder
-  init(url:settings:) 

Initializer

# init(url:settings:)

Creates an audio recorder with settings.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    url: URL,
    settings: [String : Any]
) throws
```

## Parameters 

`url`  

The file system location to record to.

`settings`  

The audio settings to use for the recording.

## Return Value

A new audio recorder, or nil if an error occurred.

## Discussion

The system supports the following keys when defining the format settings:

| Key | Supported Values |
|----|----|
| AVFormatIDKey | kAudioFormatLinearPCM  kAudioFormatMPEG4AAC  kAudioFormatAppleLossless  kAudioFormatAppleIMA4  kAudioFormatiLBC  kAudioFormatULaw |
| AVSampleRateKey | 8 kHz to 192 kHz |
| AVNumberOfChannelsKey | 1 to 64 |

The system supports additional configuration options based on your selected audio format. See Linear PCM Format Settings for information about customizing Linear PCM formats and Encoder Settings for compressed formats.

## See Also

### Creating an audio recorder

init(url: URL, format: AVAudioFormat) throws

Creates an audio recorder with an audio format.

