

- AVFoundation
- AVAssetVariant
- AVAssetVariant.AudioAttributes
- AVAssetVariant.AudioAttributes.RenditionSpecificAttributes
-  isBinaural 

Instance Property

# isBinaural

A Boolean value that indicates the variant is best suited for delivery to headphones.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var isBinaural: Bool { get }
```

## Discussion

A binaural variant may originate from a direct binaural recording or from the processing of a multichannel audio source.

## See Also

### Accessing Attributes

var channelCount: Int?

The count of audio channels in the rendition.

var isImmersive: Bool

A Boolean value that indicates whether this variant contains virtualized or otherwise preprocessed audio content suitable for various purposes.

var isDownmix: Bool

A Boolean value that indicates whether the variant is a downmix derivative of other media of greater channel count.

