

- AVFoundation
- AVAssetVariant
- AVAssetVariant.AudioAttributes
- AVAssetVariant.AudioAttributes.RenditionSpecificAttributes
-  channelCount 

Instance Property

# channelCount

The count of audio channels in the rendition.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@nonobjc
var channelCount: Int? { get }
```

## See Also

### Accessing Attributes

var isBinaural: Bool

A Boolean value that indicates the variant is best suited for delivery to headphones.

var isImmersive: Bool

A Boolean value that indicates whether this variant contains virtualized or otherwise preprocessed audio content suitable for various purposes.

var isDownmix: Bool

A Boolean value that indicates whether the variant is a downmix derivative of other media of greater channel count.

