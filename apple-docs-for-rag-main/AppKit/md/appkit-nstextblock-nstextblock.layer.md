

- AppKit
- NSTextBlock
-  NSTextBlock.Layer 

Enumeration

# NSTextBlock.Layer

The following constants specify values used by the properties and methods contentWidthValueType, setWidth(_:type:for:edge:), setWidth(_:type:for:), width(for:edge:), and widthValueType(for:edge:) to specify text block layer values.

macOS

``` source
enum Layer
```

## Topics

### Constants

case padding

Padding of the text block: space surrounding the content area extending to the border.

case border

The border of the text block.

case margin

Margin of the text block: space surrounding the border.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting and setting margins, borders, and padding

func setWidth(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Layer, edge: NSRectEdge)

Sets the width of a specified edge of a specified layer of the text block.

func setWidth(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Layer)

Sets the width of all edges of a specified layer of the text block.

func width(for: NSTextBlock.Layer, edge: NSRectEdge) -> CGFloat

Returns the width of an edge of a specified layer of the text block.

func widthValueType(for: NSTextBlock.Layer, edge: NSRectEdge) -> NSTextBlock.ValueType

Returns the value type of an edge of a specified layer of the text block.

