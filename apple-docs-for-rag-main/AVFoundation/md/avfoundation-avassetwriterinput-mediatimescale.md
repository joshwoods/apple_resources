

- AVFoundation
- AVAssetWriterInput
-  mediaTimeScale 

Instance Property

# mediaTimeScale

The time scale of the track in the output file.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var mediaTimeScale: CMTimeScale { get set }
```

## Discussion

The default value is `0`, which indicates that the input chooses an appropriate value, if applicable. It’s an error to set this value if the input’s media type is audio.

You can’t set this value after writing starts.

## See Also

### Configuring Presentation

var naturalSize: CGSize

The natural display dimensions of the output’s visual media.

var transform: CGAffineTransform

The transform to use for display of the output’s visual media.

var preferredVolume: Float

The volume to prefer for playback of the output’s audio data.

var marksOutputTrackAsEnabled: Bool

A Boolean value that indicates whether to enable a track in the output for playback and processing.

