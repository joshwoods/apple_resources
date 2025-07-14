

- AVFoundation
- AVAssetWriterInput
-  preferredVolume 

Instance Property

# preferredVolume

The volume to prefer for playback of the output’s audio data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var preferredVolume: Float { get set }
```

## Discussion

The default value for audio data is `1.0`, which indicates typical playback level. Set the value for this property in the range of `0.0` to `1.0`. For nonaudio media, the default value is `0.0`.

You can’t set this value after writing starts.

## See Also

### Configuring Presentation

var naturalSize: CGSize

The natural display dimensions of the output’s visual media.

var transform: CGAffineTransform

The transform to use for display of the output’s visual media.

var mediaTimeScale: CMTimeScale

The time scale of the track in the output file.

var marksOutputTrackAsEnabled: Bool

A Boolean value that indicates whether to enable a track in the output for playback and processing.

