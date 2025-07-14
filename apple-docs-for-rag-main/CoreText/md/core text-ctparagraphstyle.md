

- Core Text
-  CTParagraphStyle 

Class

# CTParagraphStyle

Paragraph or ruler attributes in an attributed string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CTParagraphStyle
```

## Overview

A paragraph style object represents a complex attribute value in an attributed string, storing a number of subattributes that affect paragraph layout for the characters of the string. Among these subattributes are alignment, tab stops, writing direction, line-breaking mode, and indentation settings.

## Topics

### Creating Paragraph Styles

func CTParagraphStyleCreate(UnsafePointer&lt;CTParagraphStyleSetting>?, Int) -> CTParagraphStyle

Creates an immutable paragraph style.

func CTParagraphStyleCreateCopy(CTParagraphStyle) -> CTParagraphStyle

Creates an immutable copy of a paragraph style.

### Getting the Value of a Style Specifier

func CTParagraphStyleGetValueForSpecifier(CTParagraphStyle, CTParagraphStyleSpecifier, Int, UnsafeMutableRawPointer) -> Bool

Obtains the current value for a single setting specifier.

### Getting the Type Identifier

func CTParagraphStyleGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier of the paragraph style object.

### Data Types

struct CTParagraphStyleSetting

This structure is used to alter the paragraph style.

### Constants

enum CTTextAlignment

Constants that specify text alignment.

enum CTLineBreakMode

These constants specify what happens when a line is too long for its frame.

enum CTWritingDirection

These constants specify the writing direction.

enum CTParagraphStyleSpecifier

Constants used to query and modify a paragraph style object.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Opaque Types

class CTFont

A font object.

class CTFontCollection

A font collection.

class CTFontDescriptor

A font descriptor.

class CTFrame

A frame.

class CTFramesetter

Generate text frames.

class CTGlyphInfo

Override a font’s specified mapping from Unicode to the glyph ID.

class CTLine

A line of text.

class CTRun

A glyph run.

class CTRunDelegate

A run delegate.

class CTTextTab

A tab in a paragraph style, storing an alignment type and location.

class CTTypesetter

A typesetter which performs line layout.

