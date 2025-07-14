

- AVFoundation
- AVAssetWriterInput
-  transform 

Instance Property

# transform

The transform to use for display of the output’s visual media.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var transform: CGAffineTransform { get set }
```

## Discussion

By default, the input uses the CGAffineTransformIdentity transform.

You can’t set this value after writing starts.

## See Also

### Configuring Presentation

var naturalSize: CGSize

The natural display dimensions of the output’s visual media.

var preferredVolume: Float

The volume to prefer for playback of the output’s audio data.

var mediaTimeScale: CMTimeScale

The time scale of the track in the output file.

var marksOutputTrackAsEnabled: Bool

A Boolean value that indicates whether to enable a track in the output for playback and processing.

