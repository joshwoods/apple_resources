

- AVFoundation
- AVAssetVariant
-  audioAttributes 

Instance Property

# audioAttributes

The audio rendition attributes for the variant.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var audioAttributes: AVAssetVariant.AudioAttributes? { get }
```

## Discussion

This property value is `nil` if the variant defines no audio attributes.

## See Also

### Configuring Attributes

class AudioAttributes

An object that defines the audio attributes for an asset variant.

var videoAttributes: AVAssetVariant.VideoAttributes?

The video rendition attributes for the variant.

class VideoAttributes

An object that defines the video attributes for an asset variant.

