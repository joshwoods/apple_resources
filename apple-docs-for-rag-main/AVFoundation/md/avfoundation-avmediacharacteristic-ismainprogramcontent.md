

- AVFoundation
- AVMediaCharacteristic
-  isMainProgramContent 

Type Property

# isMainProgramContent

A media characteristic that indicates a track or media selection option includes content its author indicates is essential to the asset’s presentation.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
static let isMainProgramContent: AVMediaCharacteristic
```

## Discussion

Example: an option that presents the main program audio for the presentation, regardless of locale, would typically have this characteristic.

The value of this characteristic is `public.main-program-content`.

The system infers the presence of this characteristic for a media option; it considers any option that doesn’t have the characteristic isAuxiliaryContent to be main content.

## See Also

### Content

static let isOriginalContent: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option contains original content.

static let isAuxiliaryContent: AVMediaCharacteristic

A media characteristic that indicates a track or media selection option includes content its author indicates is auxiliary to the asset’s presentation.

