

- AVFoundation
- AVPlayerItemLegibleOutput
-  AVPlayerItemLegibleOutput.TextStylingResolution 

Structure

# AVPlayerItemLegibleOutput.TextStylingResolution

A text styling resolution.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct TextStylingResolution
```

## Topics

### Text Styling Options

static let `default`: AVPlayerItemLegibleOutput.TextStylingResolution

The text styling information is the same level of information that AVFoundation uses within a player layer.

static let sourceAndRulesOnly: AVPlayerItemLegibleOutput.TextStylingResolution

The level of resolution excludes styling provided by the user-level Media Accessibility settings.

### Initializers

init(rawValue: String)

Creates a text styling resolution structure with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Text Styling

var textStylingResolution: AVPlayerItemLegibleOutput.TextStylingResolution

A string identifier indicating the degree of text styling to be applied to attributed strings vended by the object.

