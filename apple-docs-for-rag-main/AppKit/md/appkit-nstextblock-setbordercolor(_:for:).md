

- AppKit
- NSTextBlock
-  setBorderColor(\_:for:) 

Instance Method

# setBorderColor(\_:for:)

Sets the border color of the specified edge of the text block.

macOS

``` source
func setBorderColor(
    _ color: NSColor?,
    for edge: NSRectEdge
)
```

## Parameters 

`color`  

The new color.

`edge`  

The edge whose color is to be set.

## Discussion

This setting has no visible effect unless the border width is larger than the default, which is 0.

## See Also

### Related Documentation

func setWidth(CGFloat, type: NSTextBlock.ValueType, for: NSTextBlock.Layer)

Sets the width of all edges of a specified layer of the text block.

### Working with color

var backgroundColor: NSColor?

The background color of the text block.

func setBorderColor(NSColor?)

Sets the color of all borders of the text block.

func borderColor(for: NSRectEdge) -> NSColor?

Returns the border color of the specified text block edge.

