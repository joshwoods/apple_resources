

- AVFoundation
- AVAssetVariant
- AVAssetVariant.AudioAttributes
- AVAssetVariant.AudioAttributes.RenditionSpecificAttributes
-  isImmersive 

Instance Property

# isImmersive

A Boolean value that indicates whether this variant contains virtualized or otherwise preprocessed audio content suitable for various purposes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var isImmersive: Bool { get }
```

## Discussion

If a variant audio redition is immersive it’s eligible for rendering to headphones or speakers.

## See Also

### Accessing Attributes

var channelCount: Int?

The count of audio channels in the rendition.

var isBinaural: Bool

A Boolean value that indicates the variant is best suited for delivery to headphones.

var isDownmix: Bool

A Boolean value that indicates whether the variant is a downmix derivative of other media of greater channel count.

