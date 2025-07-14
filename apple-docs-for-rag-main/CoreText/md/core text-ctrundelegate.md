

- Core Text
-  CTRunDelegate 

Class

# CTRunDelegate

A run delegate.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CTRunDelegate
```

## Overview

A run delegate is assigned to a run (attribute range) to control typographic traits such glyph ascent, glyph descent, and glyph width.

The callbacks defined for `CTRunDelegate` objects are provided by the owner of a run delegate and are used to modify glyph metrics during layout. The values returned by the delegate are applied to each glyph in the run or runs corresponding to the attribute with that delegate.

## Topics

### Creating a Run Delegate

func CTRunDelegateCreate(UnsafePointer&lt;CTRunDelegateCallbacks>, UnsafeMutableRawPointer?) -> CTRunDelegate?

Creates an immutable instance of a run delegate.

### Getting Information About a Run Delegate

func CTRunDelegateGetRefCon(CTRunDelegate) -> UnsafeMutableRawPointer

Returns a run delegate’s “refCon” value.

func CTRunDelegateGetTypeID() -> CFTypeID

Returns the type of CTRunDelegate objects.

### Callbacks

typealias CTRunDelegateGetAscentCallback

Defines a pointer to a function that determines typographic ascent of glyphs in the run.

typealias CTRunDelegateGetDescentCallback

Defines a pointer to a function that determines typographic descent of glyphs in the run.

typealias CTRunDelegateGetWidthCallback

Defines a pointer to a function that determines the typographic width of glyphs in the run.

typealias CTRunDelegateDeallocateCallback

Defines a pointer to a function that is invoked when a CTRunDelegate object is deallocated.

### Data Types

struct CTRunDelegateCallbacks

A structure holding pointers to callbacks implemented by the run delegate.

### Constants

Run Delegate Versions

The version of the run delegate.

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

class CTParagraphStyle

Paragraph or ruler attributes in an attributed string.

class CTRun

A glyph run.

class CTTextTab

A tab in a paragraph style, storing an alignment type and location.

class CTTypesetter

A typesetter which performs line layout.

