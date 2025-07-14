

- AppKit
- NSTextBlock
-  widthValueType(for:edge:) 

Instance Method

# widthValueType(for:edge:)

Returns the value type of an edge of a specified layer of the text block.

macOS

``` source
func widthValueType(
    for layer: NSTextBlock.Layer,
    edge: NSRectEdge
) -> NSTextBlock.ValueType
```

## Parameters 

`layer`  

The layer to examine.

`edge`  

The edge of the layer to examine.

## Return Value

The value type of the `edge` of `layer`. This determines how the value for this `edge` of `layer` should be interpreted.

## See Also

### Getting and setting margins, borders, and padding

func setWidth(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Layer, edge: NSRectEdge)

Sets the width of a specified edge of a specified layer of the text block.

func setWidth(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Layer)

Sets the width of all edges of a specified layer of the text block.

func width(for: NSTextBlock.Layer, edge: NSRectEdge) -> CGFloat

Returns the width of an edge of a specified layer of the text block.

enum Layer

The following constants specify values used by the properties and methods contentWidthValueType, setWidth(_:type:for:edge:), setWidth(_:type:for:), width(for:edge:), and widthValueType(for:edge:) to specify text block layer values.

