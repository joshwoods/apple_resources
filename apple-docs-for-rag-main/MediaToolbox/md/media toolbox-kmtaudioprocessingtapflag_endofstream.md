

- Media Toolbox
-  kMTAudioProcessingTapFlag_EndOfStream 

Global Variable

# kMTAudioProcessingTapFlag_EndOfStream

Signifies that the source audio is past the end of stream.

iOS 6.0+iPadOS 6.0+Mac Catalyst 6.0+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var kMTAudioProcessingTapFlag_EndOfStream: MTAudioProcessingTapFlags { get }
```

## Discussion

This happens when the audio queue is being stopped asynchronously and has finished playing all of its data. Returned from GetSourceAudio and should be propagated on return from the process callback.

## See Also

### Flags

var kMTAudioProcessingTapFlag_StartOfStream: MTAudioProcessingTapFlags

Signifies that the source audio is the beginning of a continuous stream.

