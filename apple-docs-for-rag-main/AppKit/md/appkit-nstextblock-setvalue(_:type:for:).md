

- AppKit
- NSTextBlock
-  setValue(\_:type:for:) 

Instance Method

# setValue(\_:type:for:)

Sets a dimension of the text block.

macOS

``` source
func setValue(
    _ val: CGFloat,
    type: NSTextBlock.ValueType,
    for dimension: NSTextBlock.Dimension
)
```

## Parameters 

`val`  

The new value for the dimension.

`type`  

The type of value being provided. This controls how `val` is interpreted.

`dimension`  

The dimension to set.

## See Also

### Working with dimensions of content

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

