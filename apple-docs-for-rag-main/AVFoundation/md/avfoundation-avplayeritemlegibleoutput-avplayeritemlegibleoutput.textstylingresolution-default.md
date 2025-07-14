

- AVFoundation
- AVPlayerItemLegibleOutput
- AVPlayerItemLegibleOutput.TextStylingResolution
-  default 

Type Property

# default

The text styling information is the same level of information that AVFoundation uses within a player layer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
static let `default`: AVPlayerItemLegibleOutput.TextStylingResolution
```

## Discussion

Specify this level of text styling resolution to receive attributed strings from an `AVPlayerItemLegibleOutput` that include the same level of styling information that AVFoundation would use itself to render text within an AVPlayerLayer. The text styling will accommodate user-level Media Accessibility settings.

## See Also

### Text Styling Options

static let sourceAndRulesOnly: AVPlayerItemLegibleOutput.TextStylingResolution

The level of resolution excludes styling provided by the user-level Media Accessibility settings.

