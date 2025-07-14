

- AppKit
- NSTextBlock
-  width(for:edge:) 

Instance Method

# width(for:edge:)

Returns the width of an edge of a specified layer of the text block.

macOS

``` source
func width(
    for layer: NSTextBlock.Layer,
    edge: NSRectEdge
) -> CGFloat
```

## Parameters 

`layer`  

The layer to examine.

`edge`  

The edge of the layer to examine.

## Return Value

The width of the `edge` of `layer`. This value must be interpreted according to the value type returned by widthValueType(for:edge:).

## See Also

### Getting and setting margins, borders, and padding

func setWidth(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Layer, edge: NSRectEdge)

Sets the width of a specified edge of a specified layer of the text block.

func setWidth(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Layer)

Sets the width of all edges of a specified layer of the text block.

func widthValueType(for: NSTextBlock.Layer, edge: NSRectEdge) -> NSTextBlock.ValueType

Returns the value type of an edge of a specified layer of the text block.

enum Layer

The following constants specify values used by the properties and methods contentWidthValueType, setWidth(_:type:for:edge:), setWidth(_:type:for:), width(for:edge:), and widthValueType(for:edge:) to specify text block layer values.

