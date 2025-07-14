

- AVFoundation
- AVAssetVariant
- AVAssetVariant.AudioAttributes
-  formatIDs 

Instance Property

# formatIDs

The audio formats of the renditions present in the variant.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@nonobjc
var formatIDs: [AudioFormatID] { get }
```

## See Also

### Inspecting Audio Attributes

func renditionSpecificAttributes(for: AVMediaSelectionOption) -> AVAssetVariant.AudioAttributes.RenditionSpecificAttributes?

Returns specific attributes for the media option.

class RenditionSpecificAttributes

An object that represents attributes specific to a particular rendition.

