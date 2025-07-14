

- AVFoundation
- AVAssetVariant
- AVAssetVariant.AudioAttributes
-  renditionSpecificAttributes(for:) 

Instance Method

# renditionSpecificAttributes(for:)

Returns specific attributes for the media option.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func renditionSpecificAttributes(for mediaSelectionOption: AVMediaSelectionOption) -> AVAssetVariant.AudioAttributes.RenditionSpecificAttributes?
```

## Parameters 

`mediaSelectionOption`  

The media option for which to retrieve attributes.

## Return Value

Attributes for the rendition, or `nil` of none exist.

## See Also

### Inspecting Audio Attributes

var formatIDs: [AudioFormatID]

The audio formats of the renditions present in the variant.

class RenditionSpecificAttributes

An object that represents attributes specific to a particular rendition.

