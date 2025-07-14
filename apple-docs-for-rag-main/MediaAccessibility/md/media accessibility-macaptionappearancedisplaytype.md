

- Media Accessibility
-  MACaptionAppearanceDisplayType 

Enumeration

# MACaptionAppearanceDisplayType

A value that specifies the type of captions to display.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
enum MACaptionAppearanceDisplayType
```

## Topics

### Constants

case forcedOnly

Do not display captions unless they are forced for translation.

case automatic

If the language of the audio track differs from the system locale, then captions matching the system locale should be displayed (if available). If the language of the audio and the language of the system locale match, no captions are shown.

case alwaysOn

The most robust available captioning track should always be displayed, whether subtitles, CC, or SDH. This option is selected by a switch labeled “Closed Captions + SDH” (on the Subtitles & Captioning page of iOS) and “Prefer Closed Captions and SDH” checkbox (on the Captions pane of the Accessibility options in macOS).

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum MACaptionAppearanceDomain

A value that specifies which domain to retrieve a preference setting from.

enum MACaptionAppearanceBehavior

A value that indicates the preferred behavior for a preference setting.

enum MACaptionAppearanceFontStyle

A value that specifies a font style.

enum MACaptionAppearanceTextEdgeStyle

A value that specifies a style for the outside of the text.

