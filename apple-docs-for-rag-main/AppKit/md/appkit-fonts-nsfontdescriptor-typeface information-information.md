

- AppKit
- Fonts
- NSFontDescriptor
-  Typeface Information 

API Collection

# Typeface Information

Constants for type faces such as italic or bold.

## Overview

Typeface information is specified by the lower 16 bits of `NSFontSymbolicTraits` using the following constants.

## Topics

### Constants

var NSFontItalicTrait: Int

The font’s typestyle is italic.

var NSFontBoldTrait: Int

The font’s typestyle is boldface.

var NSFontExpandedTrait: Int

The font’s typestyle is expanded. Expanded and condensed traits are mutually exclusive.

var NSFontCondensedTrait: Int

The font’s typestyle is condensed. Expanded and condensed traits are mutually exclusive.

var NSFontMonoSpaceTrait: Int

The font uses fixed-pitch glyphs if available. The font may have multiple glyph advances (many CJK glyphs contain two spaces).

var NSFontVerticalTrait: Int

The font uses vertical glyph variants and metrics.

var NSFontUIOptimizedTrait: Int

The font synthesizes appropriate attributes for user interface rendering, such as control titles, if necessary.

## See Also

### Getting the Font Attributes

var fontAttributes: [NSFontDescriptor.AttributeName : Any]

The receiver’s dictionary of attributes.

func object(forKey: NSFontDescriptor.AttributeName) -> Any?

Returns the font attribute specified by the given key.

struct AttributeName

Constants for the names of font attributes.

struct SymbolicTraits

A symbolic description of the stylistic aspects of a font.

var matrix: AffineTransform?

The current transform matrix of the receiver.

var pointSize: CGFloat

The point size of the receiver.

var postscriptName: String?

The PostScript name of the receiver.

struct FeatureKey

Constants to use as keys to retrieve information about a font descriptor from its feature dictionary.

typealias NSFontFamilyClass

Constants that classify certain stylistic qualities of the font.

var NSFontFamilyClassMask: UInt32

Constant you use to access `NSFontFamilyClass` values in the upper four bits of `NSFontSymbolicTraits`.

struct VariationKey

Constants that can be used as keys to retrieve information about a font descriptor from its variation axis dictionary.

