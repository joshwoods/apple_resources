

- Core Text
-  CTFontStylisticClass 

Structure

# CTFontStylisticClass

The stylistic class values of the font.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CTFontStylisticClass
```

## Overview

`CTFontStylisticClass` identifies certain stylistic qualities of the font. These values correspond closely to the font class values in the OpenType OS/2 table. The class values are bundled in the upper four bits of the CTFontSymbolicTraits and can be obtained via classMaskTrait.

## Topics

### Initializers

init(rawValue: UInt32)

Creates a stylistic class structure with the specified raw value.

### Stylistic Classes

static var classOldStyleSerifs: CTFontStylisticClass

A font style based on the Latin printing style of the 15th to 17th century.

static var classTransitionalSerifs: CTFontStylisticClass

A font style based on the Latin printing style of the 18th to 19th century.

static var classModernSerifs: CTFontStylisticClass

A font style based on the Latin printing style of the 20th century.

static var classClarendonSerifs: CTFontStylisticClass

A font style variation of the Oldstyle Serifs and the Transitional Serifs.

static var classSlabSerifs: CTFontStylisticClass

A font style characterized by serifs with a square transition between the strokes and the serifs (no brackets).

static var classFreeformSerifs: CTFontStylisticClass

A font style that includes serifs but expresses a design freedom that doesn’t generally fit within the other serif design classifications.

static var classSansSerif: CTFontStylisticClass

A font style that includes most basic letter forms (excluding Scripts and Ornamentals) that do not have serifs on the strokes.

static var classOrnamentals: CTFontStylisticClass

A font style that includes highly decorated or stylized character shapes such as those typically used in headlines.

static var classScripts: CTFontStylisticClass

A font style among those typefaces designed to simulate handwriting.

static var classSymbolic: CTFontStylisticClass

A generally design-independent font style.

### Deprecated Constants

static var oldStyleSerifsClass: CTFontStylisticClass

The font’s style is based on the Latin printing style of the 15th to 17th century.

Deprecated

static var transitionalSerifsClass: CTFontStylisticClass

The font’s style is based on the Latin printing style of the 18th to 19th century.

Deprecated

static var modernSerifsClass: CTFontStylisticClass

The font’s style is based on the Latin printing style of the 20th century.

Deprecated

static var clarendonSerifsClass: CTFontStylisticClass

The font’s style is a variation of the Oldstyle Serifs and the Transitional Serifs.

Deprecated

static var slabSerifsClass: CTFontStylisticClass

The font’s style is characterized by serifs with a square transition between the strokes and the serifs (no brackets).

Deprecated

static var freeformSerifsClass: CTFontStylisticClass

The font’s style includes serifs but expresses a design freedom that doesn’t generally fit within the other serif design classifications.

Deprecated

static var sansSerifClass: CTFontStylisticClass

The font’s style includes most basic letter forms (excluding Scripts and Ornamentals) that do not have serifs on the strokes.

Deprecated

static var ornamentalsClass: CTFontStylisticClass

The font’s style includes highly decorated or stylized character shapes such as those typically used in headlines.

Deprecated

static var scriptsClass: CTFontStylisticClass

The font’s style is among those typefaces designed to simulate handwriting.

Deprecated

static var symbolicClass: CTFontStylisticClass

The font’s style is generally design independent.

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

struct CTFontSymbolicTraits

The symbolic representation of stylistic font attributes.

