

- AppKit
-  NSTextBlock 

Class

# NSTextBlock

A block of text laid out in a subregion of the text container.

macOS

``` source
class NSTextBlock
```

## Overview

A text block appears as an attribute of a paragraph, and as part of the paragraph style. The most important subclass of NSTextBlock is NSTextTableBlock, which represents a block of text that appears as a cell in a table. The table itself is a NSTextTable object. All NSTextBlock objects reference this table, which controls their sizing and positioning.

## Topics

### Creating text blocks

init()

Initializes and returns an empty text block object.

### Working with dimensions of content

func setValue(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Dimension)

Sets a dimension of the text block.

func value(for: NSTextBlock.Dimension) -> CGFloat

Returns the value of the specified text block dimension.

func valueType(for: NSTextBlock.Dimension) -> NSTextBlock.ValueType

Returns the value type of the specified text block dimension.

func setContentWidth(CGFloat, type: NSTextBlock.ValueType)

Sets the width of the text block.

var contentWidth: CGFloat

The width of the text block.

var contentWidthValueType: NSTextBlock.ValueType

The type of value stored for the text block width.

enum Dimension

The following constants specify values used by the methods setValue(_:type:for:), value(for:), and valueType(for:) to specify text block dimensions.

enum ValueType

The following constants specify values used by the methods setValue(_:type:for:) and valueType(for:) to specify text block value types.

### Getting and setting margins, borders, and padding

func setWidth(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Layer, edge: NSRectEdge)

Sets the width of a specified edge of a specified layer of the text block.

func setWidth(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Layer)

Sets the width of all edges of a specified layer of the text block.

func width(for: NSTextBlock.Layer, edge: NSRectEdge) -> CGFloat

Returns the width of an edge of a specified layer of the text block.

func widthValueType(for: NSTextBlock.Layer, edge: NSRectEdge) -> NSTextBlock.ValueType

Returns the value type of an edge of a specified layer of the text block.

enum Layer

The following constants specify values used by the properties and methods contentWidthValueType, setWidth(_:type:for:edge:), setWidth(_:type:for:), width(for:edge:), and widthValueType(for:edge:) to specify text block layer values.

### Getting and setting alignment

var verticalAlignment: NSTextBlock.VerticalAlignment

The vertical alignment of the text block.

enum VerticalAlignment

The following constants specify values used by the property verticalAlignment to specify vertical alignment.

### Working with color

var backgroundColor: NSColor?

The background color of the text block.

func setBorderColor(NSColor?, for: NSRectEdge)

Sets the border color of the specified edge of the text block.

func setBorderColor(NSColor?)

Sets the color of all borders of the text block.

func borderColor(for: NSRectEdge) -> NSColor?

Returns the border color of the specified text block edge.

### Determining size and position of a text block

func rectForLayout(at: NSPoint, in: NSRect, textContainer: NSTextContainer, characterRange: NSRange) -> NSRect

Returns the rectangle within which glyphs should be laid out for the specified arguments.

func boundsRect(forContentRect: NSRect, in: NSRect, textContainer: NSTextContainer, characterRange: NSRange) -> NSRect

Returns the rectangle the text in the block actually occupies, including padding, borders, and margins.

### Drawing colors and decorations

func drawBackground(withFrame: NSRect, in: NSView, characterRange: NSRange, layoutManager: NSLayoutManager)

Called by the layout manager to draw any colors and other decorations before the text is drawn.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSTextTable
- NSTextTableBlock

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

class NSTextTable

An object that represents a text table as a whole.

class NSTextTableBlock

A text block that appears as a cell in a text table.

