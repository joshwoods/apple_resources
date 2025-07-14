

- AppKit
- NSTextBlock
-  value(for:) 

Instance Method

# value(for:)

Returns the value of the specified text block dimension.

macOS

``` source
func value(for dimension: NSTextBlock.Dimension) -> CGFloat
```

## Return Value

The value for the specified dimension. This value should be interpreted according to the value type returned by valueType(for:).

## See Also

### Working with dimensions of content

func setValue(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Dimension)

Sets a dimension of the text block.

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

