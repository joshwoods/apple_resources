

- AVFoundation
- AVAssetWriterInput
-  init(mediaType:outputSettings:) 

Initializer

# init(mediaType:outputSettings:)

Creates an input to append sample buffers of the specified type to the output file.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    mediaType: AVMediaType,
    outputSettings: [String : Any]?
)
```

## Parameters 

`mediaType`  

The media type of the samples the input accepts.

`outputSettings`  

The settings to use for encoding the media you append to the output. Create an output settings dictionary manually, or use AVOutputSettingsAssistant to create preset-based settings.

## Discussion

If you’re appending samples that are already in an acceptable compressed format, pass a value of `nil` for the output settings to pass the buffers to the output unaltered. However, if you’re not writing to a QuickTime movie file, an asset writer only supports passing through a restricted set of media types and subtypes. To pass through media data to files with a type other than mov, pass a nonnull format hint using the init(mediaType:outputSettings:sourceFormatHint:) instead.

### Configuring Audio Settings

You must fully specify the audio settings dictionary when using this initializer, which means you must provide values for the following keys:

- AVFormatIDKey. The identifier of the audio format. For kAudioFormatLinearPCM format, you must include values for all relevant keys with a `AVLinearPCM` prefix, and for kAudioFormatAppleLossless, you must specify a value for AVEncoderBitDepthHintKey.

- AVSampleRateKey. The sample rate of the audio. Common values are `44100` and `48000`.

- AVNumberOfChannelsKey. If no other channel layout information is available, specifying a value of `1` results in mono output and a value of `2` results in stereo output. If AVNumberOfChannelsKey specifies a channel count greater than `2`, the dictionary must also specify a value for AVChannelLayoutKey.

Note

The system doesn’t support specifying a value for AVSampleRateConverterAudioQualityKey in audio output settings.

### Configuring Video Settings

A video output settings dictionary must request a compressed video format, which means that the value you specify must follow the rules for compressed video output.

You must fully specify the video settings dictionary when using this initializer, which means you must provide values for the following keys AVVideoCodecKey, AVVideoWidthKey, AVVideoHeightKey.

Note

Specifying a AVVideoScalingModeKey value of AVVideoScalingModeFit results in an error.

## See Also

### Creating an Input

init(mediaType: AVMediaType, outputSettings: [String : Any]?, sourceFormatHint: CMFormatDescription?)

Creates an input that appends sample buffers of the specified type and format hint to the output file.

