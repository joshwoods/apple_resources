

- AppKit
- NSTextBlock
-  setWidth(\_:type:for:edge:) 

Instance Method

# setWidth(\_:type:for:edge:)

Sets the width of a specified edge of a specified layer of the text block.

macOS

``` source
func setWidth(
    _ val: CGFloat,
    type: NSTextBlock.ValueType,
    for layer: NSTextBlock.Layer,
    edge: NSRectEdge
)
```

## Parameters 

`val`  

The new value for the specified edge width.

`type`  

The type of value being provided. This controls how `val` is interpreted.

`layer`  

The layer of the text block to modify.

`edge`  

The edge of the layer to modify.

## See Also

### Getting and setting margins, borders, and padding

func setWidth(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Layer)

Sets the width of all edges of a specified layer of the text block.

func width(for: NSTextBlock.Layer, edge: NSRectEdge) -> CGFloat

Returns the width of an edge of a specified layer of the text block.

func widthValueType(for: NSTextBlock.Layer, edge: NSRectEdge) -> NSTextBlock.ValueType

Returns the value type of an edge of a specified layer of the text block.

enum Layer

The following constants specify values used by the properties and methods contentWidthValueType, setWidth(_:type:for:edge:), setWidth(_:type:for:), width(for:edge:), and widthValueType(for:edge:) to specify text block layer values.

