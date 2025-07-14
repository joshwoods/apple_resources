

- AppKit
-  NSGlyphStorage 

Protocol

# NSGlyphStorage

A set of methods that a glyph storage object must implement to interact properly with NSGlyphGenerator.

macOS

``` source
protocol NSGlyphStorage
```

## Overview

An example of a class that conforms to the NSGlyphStorage protocol is NSLayoutManager.

## Topics

### Returning text storage

func attributedString() -> NSAttributedString

Returns the text storage object from which the `NSGlyphGenerator` object procures characters for glyph generation.

**Required**

### Returning glyph display options

func layoutOptions() -> Int

Returns the current layout options.

**Required**

### Modifying the glyph cache

func insertGlyphs(UnsafePointer&lt;NSGlyph>, length: Int, forStartingGlyphAt: Int, characterIndex: Int)

Inserts the given glyphs into the glyph cache and maps them to the specified characters.

**Required**

func setIntAttribute(Int, value: Int, forGlyphAt: Int)

Sets a custom attribute value for a given glyph.

**Required**

### Constants

Layout Options

Layout options returned as a bit mask by the layoutOptions() method.

## Relationships

### Conforming Types

- NSLayoutManager

## See Also

### Glyphs

typealias NSGlyph

The type used to specify glyphs.

class NSGlyphGenerator

An object that performs the initial, nominal glyph generation phase in the layout process.

class NSGlyphInfo

A glyph attribute in an attributed string.

Reserved Glyph Codes

These constants define reserved glyph codes.

enum NSFontRenderingMode

The font rendering mode.

