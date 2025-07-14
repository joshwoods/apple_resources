

- Core Text
-  CTFontSymbolicTraits 

Structure

# CTFontSymbolicTraits

The symbolic representation of stylistic font attributes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CTFontSymbolicTraits
```

## Overview

`CTFontSymbolicTraits` symbolically describes stylistic aspects of a font. The upper 16 bits are used to describe appearance of the font, whereas the lower 16 bits are for typeface information. The font appearance information represented by the upper 16 bits can be used for stylistic font matching.

## Topics

### Initializers

init(rawValue: UInt32)

Creates a symbolic traits structure with the specified raw value.

### Symbolic Traits

static var traitItalic: CTFontSymbolicTraits

The font typestyle is italic.

static var traitBold: CTFontSymbolicTraits

The font typestyle is boldface.

static var traitExpanded: CTFontSymbolicTraits

The font typestyle is expanded.

static var traitCondensed: CTFontSymbolicTraits

The font typestyle is condensed.

static var traitMonoSpace: CTFontSymbolicTraits

The font uses fixed-pitch glyphs if available.

static var traitVertical: CTFontSymbolicTraits

The font uses vertical glyph variants and metrics.

static var traitUIOptimized: CTFontSymbolicTraits

The font synthesizes appropriate attributes for user interface rendering, such as control titles, if necessary.

static var traitColorGlyphs: CTFontSymbolicTraits

The font contains color glyphs.

static var traitComposite: CTFontSymbolicTraits

The font is in Composite Font Reference format.

static var traitClassMask: CTFontSymbolicTraits

Mask for the font class.

### Deprecated Constants

static var italicTrait: CTFontSymbolicTraits

The font typestyle is italic.

Deprecated

static var boldTrait: CTFontSymbolicTraits

The font typestyle is boldface.

Deprecated

static var expandedTrait: CTFontSymbolicTraits

The font typestyle is expanded.

Deprecated

static var condensedTrait: CTFontSymbolicTraits

The font typestyle is condensed.

Deprecated

static var monoSpaceTrait: CTFontSymbolicTraits

The font uses fixed-pitch glyphs if available.

Deprecated

static var verticalTrait: CTFontSymbolicTraits

The font uses vertical glyph variants and metrics.

Deprecated

static var uiOptimizedTrait: CTFontSymbolicTraits

The font synthesizes appropriate attributes for user interface rendering, such as control titles, if necessary.

Deprecated

static var colorGlyphsTrait: CTFontSymbolicTraits

The font contains color glyphs.

Deprecated

static var compositeTrait: CTFontSymbolicTraits

The font is in Composite Font Reference format.

Deprecated

static var classMaskTrait: CTFontSymbolicTraits

Mask for the font class.

Deprecated

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

### Accessing Font Traits

Font Traits

The keys for accessing font traits from a font descriptor.

Font Class Mask Shift Constants

These constants represent the font class mask shift.

struct CTFontStylisticClass

The stylistic class values of the font.

