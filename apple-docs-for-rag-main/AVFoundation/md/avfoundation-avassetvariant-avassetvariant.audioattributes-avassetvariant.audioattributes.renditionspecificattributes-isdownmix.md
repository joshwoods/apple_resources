

- AVFoundation
- AVAssetVariant
- AVAssetVariant.AudioAttributes
- AVAssetVariant.AudioAttributes.RenditionSpecificAttributes
-  isDownmix 

Instance Property

# isDownmix

A Boolean value that indicates whether the variant is a downmix derivative of other media of greater channel count.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var isDownmix: Bool { get }
```

## Discussion

If the stream provides one or more multichannel variants, the system assumes the dowmix rendition to be compatible in its internal timing and other attributes with the other variants. Typically, this is because the variant derives its content from the same source. You can use a downmix as a suitable substitute for a multichannel variant under some conditions.

## See Also

### Accessing Attributes

var channelCount: Int?

The count of audio channels in the rendition.

var isBinaural: Bool

A Boolean value that indicates the variant is best suited for delivery to headphones.

var isImmersive: Bool

A Boolean value that indicates whether this variant contains virtualized or otherwise preprocessed audio content suitable for various purposes.

