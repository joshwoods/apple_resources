

- AVFoundation
- AVAssetReaderAudioMixOutput
-  init(audioTracks:audioSettings:) 

Initializer

# init(audioTracks:audioSettings:)

Creates an object that reads mixed audio from the specified audio tracks.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
init(
    audioTracks: [AVAssetTrack],
    audioSettings: [String : Any]?
)
```

## Parameters 

`audioTracks`  

An array of track objects of type audio from which to source the sample buffers to mix.

`audioSettings`  

Optional audio settings to use for audio output. Pass `nil` to receive the decoded samples in an uncompressed format. To determine the specific format, examine the value of the sample buffer’s formatDescription property.

For non-`nil` audio settings, the dictionary must contain values for the Linear PCM Format Settings keys. The output doesn’t support the AVSampleRateConverterAudioQualityKey constant.

