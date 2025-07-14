

- AppKit
-  NSTextTable 

Class

# NSTextTable

An object that represents a text table as a whole.

macOS

``` source
class NSTextTable
```

## Overview

A text table is responsible for laying out and drawing the text table blocks it contains, and it maintains the basic parameters of the table.

## Topics

### Getting and setting number of columns

var numberOfColumns: Int

The number of columns in the text table.

### Getting and setting layout algorithm

var layoutAlgorithm: NSTextTable.LayoutAlgorithm

The text table layout algorithm.

### Collapsing borders

var collapsesBorders: Bool

A Boolean value indicating whether the text table borders are collapsible.

### Hiding empty cells

var hidesEmptyCells: Bool

A Boolean value indicating whether the text table hides empty cells.

### Determining layout rectangles

func rect(for: NSTextTableBlock, layoutAt: NSPoint, in: NSRect, textContainer: NSTextContainer, characterRange: NSRange) -> NSRect

Returns the rectangle within which glyphs should be laid out for a text table block.

func boundsRect(for: NSTextTableBlock, contentRect: NSRect, in: NSRect, textContainer: NSTextContainer, characterRange: NSRange) -> NSRect

Returns the rectangle the text table block actually occupies, including padding, borders, and margins.

### Drawing the table

func drawBackground(for: NSTextTableBlock, withFrame: NSRect, in: NSView, characterRange: NSRange, layoutManager: NSLayoutManager)

Draws any colors and other decorations for a text table block.

### Constants

enum LayoutAlgorithm

These constants, specifying the type of text table layout algorithm, are used with layoutAlgorithm.

## Relationships

### Inherits From

- NSTextBlock

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Formatting and attributes

class NSParagraphStyle

The paragraph or ruler attributes for an attributed string.

class NSMutableParagraphStyle

An object for changing the values of the subattributes in a paragraph style attribute.

class NSTextTab

A tab in a paragraph.

class NSTextList

A section of text that forms a single list.

class NSTextTableBlock

A text block that appears as a cell in a text table.

class NSTextBlock

A block of text laid out in a subregion of the text container.

