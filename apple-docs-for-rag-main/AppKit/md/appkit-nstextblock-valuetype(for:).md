

- AppKit
- NSTextBlock
-  valueType(for:) 

Instance Method

# valueType(for:)

Returns the value type of the specified text block dimension.

macOS

``` source
func valueType(for dimension: NSTextBlock.Dimension) -> NSTextBlock.ValueType
```

## Return Value

The value type for the specified text block dimension. This result determines how the value for the dimension should be interpreted.

## See Also

### Working with dimensions of content

func setValue(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Dimension)

Sets a dimension of the text block.

func value(for: NSTextBlock.Dimension) -> CGFloat

Returns the value of the specified text block dimension.

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

