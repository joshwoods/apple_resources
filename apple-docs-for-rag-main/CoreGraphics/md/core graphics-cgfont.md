

- Core Graphics
-  CGFont 

Class

# CGFont

A set of character glyphs and layout information for drawing text.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGFont
```

## Overview

A glyph can represent a single character (such as ‘b’), more than one character (such as the “ﬁ” ligature), or a special character such as a space. Core Graphics retrieves the glyphs for the font from ATS (Apple Type Services) and paints the glyphs based on the relevant parameters of the current graphics state.

Core Graphics provides a limited, low-level interface for drawing text. For information on text-drawing functions, see CGContext. For full Unicode and text-layout support, use the services provided by TextKit).

## Topics

### Creating Font Objects

init?(CGDataProvider)

Creates a font object from data supplied from a data provider.

init?(CFString)

Creates a font object corresponding to the font specified by a PostScript or full name.

### Examining Font Metadata

var fullName: CFString?

Returns the full name associated with a font object.

### Examining Font Metrics

var ascent: Int32

Returns the ascent of a font.

var capHeight: Int32

Returns the cap height of a font.

var descent: Int32

Returns the descent of a font.

var fontBBox: CGRect

Returns the bounding box of a font.

var italicAngle: CGFloat

Returns the italic angle of a font.

var leading: Int32

Returns the leading of a font.

var stemV: CGFloat

Returns the thickness of the dominant vertical stems of glyphs in a font.

var unitsPerEm: Int32

Returns the number of glyph space units per em for the provided font.

var xHeight: Int32

Returns the x-height of a font.

### Working with PostScript Fonts

var postScriptName: CFString?

Obtains the PostScript name of a font.

func canCreatePostScriptSubset(CGFontPostScriptFormat) -> Bool

Determines whether Core Graphics can create a subset of the font in PostScript format.

func createPostScriptSubset(subsetName: CFString, format: CGFontPostScriptFormat, glyphs: UnsafePointer&lt;CGGlyph>?, count: Int, encoding: UnsafePointer&lt;CGGlyph>?) -> CFData?

Creates a subset of the font in the specified PostScript format.

enum CGFontPostScriptFormat

Possible formats for a PostScript font subset.

func createPostScriptEncoding(encoding: UnsafePointer&lt;CGGlyph>?) -> CFData?

Creates a PostScript encoding of a font.

### Working with Font Tables

var tableTags: CFArray?

Returns an array of tags that correspond to the font tables for a font.

func table(for: UInt32) -> CFData?

Returns the font table that corresponds to the provided tag.

Font Table Index Values

Possible values for an index into a font table.

Obsolete Font Table Index Values

Deprecated values for an index into a font table.

### Working with Variations

func copy(withVariations: CFDictionary?) -> CGFont?

Creates a copy of a font using a variation specification dictionary.

var variations: CFDictionary?

Returns the variation specification dictionary for a font.

var variationAxes: CFArray?

Returns an array of the variation axis dictionaries for a font.

Font Variation Axis Keys

Keys used for a font variation axis dictionary.

### Working with Glyphs

var numberOfGlyphs: Int

Returns the number of glyphs in a font.

func name(for: CGGlyph) -> CFString?

Returns the glyph name of the specified glyph in the specified font.

func getGlyphWithGlyphName(name: CFString) -> CGGlyph

Returns the glyph for the glyph name associated with the specified font object.

func getGlyphBBoxes(glyphs: UnsafePointer&lt;CGGlyph>, count: Int, bboxes: UnsafeMutablePointer&lt;CGRect>) -> Bool

Get the bounding box of each glyph in an array.

func getGlyphAdvances(glyphs: UnsafePointer&lt;CGGlyph>, count: Int, advances: UnsafeMutablePointer&lt;Int32>) -> Bool

Gets the advance width of each glyph in the provided array.

typealias CGGlyph

An index into the internal glyph table of a font.

let kCGGlyphMax: CGFontIndex

The maximum allowed value of a CGGlyph.

typealias CGFontIndex

An index into a font table.

let kCGFontIndexMax: CGFontIndex

The maximum allowed value of a CGFontIndex.

let kCGFontIndexInvalid: CGFontIndex

An invalid font index (a value which never represents a valid glyph).

### Working with Core Foundation Types

class var typeID: CFTypeID

Returns the Core Foundation type identifier for Core Graphics fonts.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Quartz 2D Programming Guide

### Colors and Fonts

class CGColor

A set of components that define a color, with a color space specifying how to interpret them.

class CGColorConversionInfo

An object that describes how to convert between color spaces for use by other system services.

class CGColorSpace

A profile that specifies how to interpret a color value for display.

