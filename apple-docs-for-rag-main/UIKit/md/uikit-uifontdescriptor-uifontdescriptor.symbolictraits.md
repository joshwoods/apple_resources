

- UIKit
- UIFontDescriptor
-  UIFontDescriptor.SymbolicTraits 

Structure

# UIFontDescriptor.SymbolicTraits

Constants that describe the stylistic aspects of a font.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
struct SymbolicTraits
```

## Overview

The lower 16 bits represent the typeface, and the upper 16 bits describe appearance of the font. The font appearance information represented by the upper 16 bits of NSFontSymbolicTraits can be used for stylistic font matching. UIFontDescriptor.Class constants classify certain stylistic qualities of the font.

## Topics

### Font traits

static var traitItalic: UIFontDescriptor.SymbolicTraits

The font’s style is italic.

static var traitBold: UIFontDescriptor.SymbolicTraits

The font’s style is boldface.

static var traitExpanded: UIFontDescriptor.SymbolicTraits

The font’s characters have an expanded width.

static var traitCondensed: UIFontDescriptor.SymbolicTraits

The font’s characters have a condensed width.

static var traitMonoSpace: UIFontDescriptor.SymbolicTraits

The font’s characters all have the same width.

static var traitVertical: UIFontDescriptor.SymbolicTraits

The font uses vertical glyph variants and metrics.

static var traitUIOptimized: UIFontDescriptor.SymbolicTraits

The font synthesizes appropriate attributes for user interface rendering, such as in control titles, if necessary.

static var traitTightLeading: UIFontDescriptor.SymbolicTraits

The font uses a leading value that’s less than the default.

static var traitLooseLeading: UIFontDescriptor.SymbolicTraits

The font uses a leading value that’s greater than the default.

static var classMask: UIFontDescriptor.SymbolicTraits

The font family class mask that you use to access font descriptor values.

static var classOldStyleSerifs: UIFontDescriptor.SymbolicTraits

The font’s characters include serifs, and reflect the Latin printing style of the 15th to 17th centuries.

static var classTransitionalSerifs: UIFontDescriptor.SymbolicTraits

The font’s characters include serifs, and reflect the Latin printing style of the 18th to 19th centuries.

static var classModernSerifs: UIFontDescriptor.SymbolicTraits

The font’s characters include serifs, and reflect the Latin printing style of the 20th century.

static var classClarendonSerifs: UIFontDescriptor.SymbolicTraits

The font’s characters include variations of old style and transitional serifs.

static var classSlabSerifs: UIFontDescriptor.SymbolicTraits

The font’s characters use square transitions, without brackets, between strokes and serifs.

static var classFreeformSerifs: UIFontDescriptor.SymbolicTraits

The font’s characters include serifs, and don’t generally fit within other serif design classifications.

static var classSansSerif: UIFontDescriptor.SymbolicTraits

The font’s characters don’t have serifs.

static var classOrnamentals: UIFontDescriptor.SymbolicTraits

The font’s characters use highly decorated or stylized character shapes.

static var classScripts: UIFontDescriptor.SymbolicTraits

The font’s characters simulate handwriting.

static var classSymbolic: UIFontDescriptor.SymbolicTraits

The font’s characters consist mainly of symbols rather than letters and numbers.

### Initializer

init(rawValue: UInt32)

Creates a symbol traits structure with the specified raw value.

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

### Fonts

Scaling Fonts Automatically

Scale text in your interface automatically using Dynamic Type.

Adding a Custom Font to Your App

Add a custom font to your app and use it in your app’s interface.

class UIFont

An object that provides access to the font’s characteristics.

class UIFontDescriptor

A collection of attributes that describes a font.

class UIFontMetrics

A utility object for obtaining custom fonts that scale to support Dynamic Type.

