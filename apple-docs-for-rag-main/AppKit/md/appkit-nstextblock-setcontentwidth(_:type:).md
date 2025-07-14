

- AppKit
- NSTextBlock
-  setContentWidth(\_:type:) 

Instance Method

# setContentWidth(\_:type:)

Sets the width of the text block.

macOS

``` source
func setContentWidth(
    _ val: CGFloat,
    type: NSTextBlock.ValueType
)
```

## Parameters 

`val`  

The new value for the width.

`type`  

The type of value being provided. This controls how `val` is interpreted.

## See Also

### Working with dimensions of content

func setValue(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Dimension)

Sets a dimension of the text block.

func value(for: NSTextBlock.Dimension) -> CGFloat

Returns the value of the specified text block dimension.

func valueType(for: NSTextBlock.Dimension) -> NSTextBlock.ValueType

Returns the value type of the specified text block dimension.

var contentWidth: CGFloat

The width of the text block.

var contentWidthValueType: NSTextBlock.ValueType

The type of value stored for the text block width.

enum Dimension

The following constants specify values used by the methods setValue(_:type:for:), value(for:), and valueType(for:) to specify text block dimensions.

enum ValueType

The following constants specify values used by the methods setValue(_:type:for:) and valueType(for:) to specify text block value types.

