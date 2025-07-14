

- Core Text
-  CTRubyOverhang 

Enumeration

# CTRubyOverhang

Constants that specify whether, and on which side, ruby text can overhang adjacent text if it’s wider than the base text.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CTRubyOverhang
```

## Topics

### Constants

case auto

The ruby text can overhang adjacent text on both sides.

case start

The ruby text can overhang the text that precedes it.

case end

The ruby text can overhang the text that follows it.

case none

The ruby text can’t overhang the preceding or following text.

case invalid

The overhang specification is invalid.

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

enum CTRubyPosition

Constants that specify the position of the ruby text relative to to the base text.

