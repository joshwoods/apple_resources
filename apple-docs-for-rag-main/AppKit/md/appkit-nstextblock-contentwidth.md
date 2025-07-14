

- AppKit
- NSTextBlock
-  contentWidth 

Instance Property

# contentWidth

The width of the text block.

macOS

``` source
var contentWidth: CGFloat { get }
```

## Discussion

This property interpreted according to the value type returned by contentWidthValueType.

## See Also

### Working with dimensions of content

func setValue(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Dimension)

Sets a dimension of the text block.

func value(for: NSTextBlock.Dimension) -> CGFloat

Returns the value of the specified text block dimension.

func valueType(for: NSTextBlock.Dimension) -> NSTextBlock.ValueType

Returns the value type of the specified text block dimension.

func setContentWidth(CGFloat, type: NSTextBlock.ValueType)

Sets the width of the text block.

var contentWidthValueType: NSTextBlock.ValueType

The type of value stored for the text block width.

enum Dimension

The following constants specify values used by the methods setValue(_:type:for:), value(for:), and valueType(for:) to specify text block dimensions.

enum ValueType

The following constants specify values used by the methods setValue(_:type:for:) and valueType(for:) to specify text block value types.

