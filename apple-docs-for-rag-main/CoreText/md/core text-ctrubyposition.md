

- Core Text
-  CTRubyPosition 

Enumeration

# CTRubyPosition

Constants that specify the position of the ruby text relative to to the base text.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CTRubyPosition
```

## Topics

### Constants

case before

The ruby text is positioned before the base text, appearing above horizontal text and to the right of vertical text.

case after

The ruby text is positioned after the base text, appearing below horizontal text and to the left of vertical text.

case interCharacter

The ruby text is positioned to the right of the base text, regardless of whether it’s horizontal or vertical.

case inline

The ruby text follows the base text with no special styling.

case count

A constant that accounts for all ruby positions during ruby annotation creation.

### Initializers

init?(rawValue: UInt8)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum CTFontDescriptorMatchingState

Constants that track the progress of font descriptor matching.

enum CTFontManagerAutoActivationSetting

Sets the auto-activation for the specified bundle identifier.

enum CTFontManagerError

Errors that prevent unregistration of fonts for a specified font file URL.

enum CTFontManagerScope

Constants that define the scope for font registration.

struct CTLineBoundsOptions

Options for getting the bounds of a line of text.

enum CTRubyAlignment

Constants that specify how to align the ruby text and the base text relative to each other when they have different lengths.

enum CTRubyOverhang

Constants that specify whether, and on which side, ruby text can overhang adjacent text if it’s wider than the base text.

