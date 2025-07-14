

- Core Text
-  CTLineBoundsOptions 

Structure

# CTLineBoundsOptions

Options for getting the bounds of a line of text.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CTLineBoundsOptions
```

## Overview

Passing `0` (no options) returns the typographic bounds, including typographic leading and shifts.

## Topics

### Line Bounds Options

static var excludeTypographicLeading: CTLineBoundsOptions

An option to exclude typographic leading.

static var excludeTypographicShifts: CTLineBoundsOptions

An option to ignore cross-stream shifts due to positioning, such as kerning or baseline alignment.

static var includeLanguageExtents: CTLineBoundsOptions

An option to include additional space based on common glyph sequences for various languages.

static var useGlyphPathBounds: CTLineBoundsOptions

An option to use glyph path bounds rather than the default typographic bounds.

static var useHangingPunctuation: CTLineBoundsOptions

An option to enable hanging punctuation.

static var useOpticalBounds: CTLineBoundsOptions

An option to use optical bounds.

### Initializers

init(rawValue: CFOptionFlags)

Creates a line bound options enumeration with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

enum CTRubyAlignment

Constants that specify how to align the ruby text and the base text relative to each other when they have different lengths.

enum CTRubyOverhang

Constants that specify whether, and on which side, ruby text can overhang adjacent text if it’s wider than the base text.

enum CTRubyPosition

Constants that specify the position of the ruby text relative to to the base text.

