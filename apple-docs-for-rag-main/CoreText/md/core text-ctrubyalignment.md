

- Core Text
-  CTRubyAlignment 

Enumeration

# CTRubyAlignment

Constants that specify how to align the ruby text and the base text relative to each other when they have different lengths.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CTRubyAlignment
```

## Topics

### Constants

case auto

Core Text automatically determines the alignment.

case start

Aligns the ruby text with the starting edge of the base text.

case center

Centers the ruby text within the width of the base text.

case end

Aligns the ruby text with the ending edge of the base text.

case distributeLetter

Distributes the ruby text evenly over the width of the base text, aligning the first and last characters of the ruby text with the first and last characters of the base text.

case distributeSpace

Distributes the ruby text evenly over the width of the base text, adding space before the first and after the last character.

case lineEdge

Aligns the ruby text to an adjacent line edge.

case invalid

The alignment is invalid.

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

enum CTRubyOverhang

Constants that specify whether, and on which side, ruby text can overhang adjacent text if it’s wider than the base text.

enum CTRubyPosition

Constants that specify the position of the ruby text relative to to the base text.

