

- AVFoundation
- AVPlayerVideoOutput
- AVPlayerVideoOutput.Configuration
-  preferredTransform 

Instance Property

# preferredTransform

The preferred transform of the visual media.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var preferredTransform: CGAffineTransform { get }
```

## Discussion

The system retrieves the transform from the AVAssetTrack that provides the media data. If the source track doesn’t specify a transform, the value of this property is CGAffineTransformIdentity.

## See Also

### Inspecting the configuration

var sourcePlayerItem: AVPlayerItem?

The player item that’s the source of this configuration.

var dataChannelDescription: [[CMTag]]

An array of data channels selected for this configuration.

var activationTime: CMTime

The host time this configuration became active on its associated player object.

