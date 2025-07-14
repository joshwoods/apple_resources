

- Core Text
-  CTTextTab 

Class

# CTTextTab

A tab in a paragraph style, storing an alignment type and location.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CTTextTab
```

## Overview

Core Text supports five alignment types: CTTextAlignment.left, CTTextAlignment.center, CTTextAlignment.right, CTTextAlignment.justified and CTTextAlignment.natural. These alignment types are absolute, not based on the line sweep direction of text.

For example, tabbed text is always positioned to the left of a right-aligned tab, whether the line sweep direction is left to right or right to left. A tab’s location, on the other hand, is relative to the back margin. A tab set at 1.5 inches, for example, is at 1.5 inches from the right in right-to-left text.

## Topics

### Creating Text Tabs

func CTTextTabCreate(CTTextAlignment, Double, CFDictionary?) -> CTTextTab

Creates and initializes a new text tab object.

### Getting Text Tab Data

func CTTextTabGetAlignment(CTTextTab) -> CTTextAlignment

Returns the text alignment of the tab.

func CTTextTabGetLocation(CTTextTab) -> Double

Returns the tab’s ruler location.

func CTTextTabGetOptions(CTTextTab) -> CFDictionary?

Returns the dictionary of attributes associated with the tab.

### Getting the Type Identifier

func CTTextTabGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier of the text tab object.

### Constants

kCTTabColumnTerminatorsAttributeName

Specifies the terminating character for a tab column.

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

class CTRunDelegate

A run delegate.

class CTTypesetter

A typesetter which performs line layout.

