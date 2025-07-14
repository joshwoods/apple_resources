

- AppKit
-  NSFontTraitMask 

Structure

# NSFontTraitMask

Constants for isolating specific traits of a font.

macOS

``` source
struct NSFontTraitMask
```

## Overview

NSFontManager categorizes fonts according to a small set of traits. You can convert fonts by adding and removing individual traits, and you can get a font with a specific combination of traits.

These pairs of traits are mutually exclusive:

- condensedFontMask and expandedFontMask

- boldFontMask and unboldFontMask

- italicFontMask and unitalicFontMask

## Topics

### Trait Masks

static var boldFontMask: NSFontTraitMask

A mask that specifies a bold font.

static var compressedFontMask: NSFontTraitMask

A mask that specifies a compressed font.

static var condensedFontMask: NSFontTraitMask

A mask that specifies a condensed font.

static var expandedFontMask: NSFontTraitMask

A mask that specifies an expanded font.

static var fixedPitchFontMask: NSFontTraitMask

A mask that specifies a fixed pitch font.

static var italicFontMask: NSFontTraitMask

A mask that specifies an italic font.

static var narrowFontMask: NSFontTraitMask

A mask that specifies a narrow font.

static var nonStandardCharacterSetFontMask: NSFontTraitMask

A mask that specifies a font containing a non-standard character set.

static var posterFontMask: NSFontTraitMask

A mask that specifies a poster-style font.

static var smallCapsFontMask: NSFontTraitMask

A mask that specifies a small-caps font.

static var unboldFontMask: NSFontTraitMask

A mask that specifies a font that is not bold.

static var unitalicFontMask: NSFontTraitMask

A mask that specifies a font that is not italic.

### Initializers

init(rawValue: UInt)

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

### Font Data

class NSFont

The representation of a font in an app.

class NSFontDescriptor

A dictionary of attributes that describe a font.

typealias NSFontFamilyClass

Constants that classify certain stylistic qualities of the font.

struct SymbolicTraits

A symbolic description of the stylistic aspects of a font.

class NSFontAssetRequest

typealias NSFontSymbolicTraits

A symbolic description of stylistic aspects of a font.

