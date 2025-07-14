

- AVFoundation
- AVAssetWriterInput
-  naturalSize 

Instance Property

# naturalSize

The natural display dimensions of the output’s visual media.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var naturalSize: CGSize { get set }
```

## Discussion

The default value is CGSizeZero, which indicates the system sets the natural size according to the dimensions of the output track’s format descriptions.

You can’t set this value after writing starts.

## See Also

### Configuring Presentation

var transform: CGAffineTransform

The transform to use for display of the output’s visual media.

var preferredVolume: Float

The volume to prefer for playback of the output’s audio data.

var mediaTimeScale: CMTimeScale

The time scale of the track in the output file.

var marksOutputTrackAsEnabled: Bool

A Boolean value that indicates whether to enable a track in the output for playback and processing.

