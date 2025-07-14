

- Media Accessibility
-  MACaptionAppearanceBehavior 

Enumeration

# MACaptionAppearanceBehavior

A value that indicates the preferred behavior for a preference setting.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
enum MACaptionAppearanceBehavior
```

## Topics

### Constants

case useValue

The preference setting should always be used.

case useContentIfAvailable

The preference setting should be used unless the content media being played has its own custom value for this setting.

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

enum MACaptionAppearanceDisplayType

A value that specifies the type of captions to display.

enum MACaptionAppearanceFontStyle

A value that specifies a font style.

enum MACaptionAppearanceTextEdgeStyle

A value that specifies a style for the outside of the text.

