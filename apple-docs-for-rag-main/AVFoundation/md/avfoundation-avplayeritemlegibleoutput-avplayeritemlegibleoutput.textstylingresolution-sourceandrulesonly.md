

- AVFoundation
- AVPlayerItemLegibleOutput
- AVPlayerItemLegibleOutput.TextStylingResolution
-  sourceAndRulesOnly 

Type Property

# sourceAndRulesOnly

The level of resolution excludes styling provided by the user-level Media Accessibility settings.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
static let sourceAndRulesOnly: AVPlayerItemLegibleOutput.TextStylingResolution
```

## Discussion

You typically use this option to override the styling specified in source media. When overriding the styling, you are strongly encouraged to allow your custom styling in turn to be overridden by user preferences for text styling that are available as Media Accessibility settings. See `Media Accessibility Function` for more information.

## See Also

### Text Styling Options

static let `default`: AVPlayerItemLegibleOutput.TextStylingResolution

The text styling information is the same level of information that AVFoundation uses within a player layer.

