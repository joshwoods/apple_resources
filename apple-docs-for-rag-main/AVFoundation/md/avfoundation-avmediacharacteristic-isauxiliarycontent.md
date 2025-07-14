

- AVFoundation
- AVMediaCharacteristic
-  isAuxiliaryContent 

Type Property

# isAuxiliaryContent

A media characteristic that indicates a track or media selection option includes content its author indicates is auxiliary to the asset’s presentation.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
static let isAuxiliaryContent: AVMediaCharacteristic
```

## Discussion

An example of auxiliary content is audio commentary about the presentation.

The value of this characteristic is `public.auxiliary-content`.

For QuickTime movies and `.m4v` files, a media option has this characteristic only if the media’s author tags it that way, or if it belongs to an alternate track group that excludes its associated track from autoselection.

## See Also

### Content

static let isOriginalContent: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option contains original content.

static let isMainProgramContent: AVMediaCharacteristic

A media characteristic that indicates a track or media selection option includes content its author indicates is essential to the asset’s presentation.

