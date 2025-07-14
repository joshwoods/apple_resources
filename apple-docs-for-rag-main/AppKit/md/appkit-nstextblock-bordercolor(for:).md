

- AppKit
- NSTextBlock
-  borderColor(for:) 

Instance Method

# borderColor(for:)

Returns the border color of the specified text block edge.

macOS

``` source
func borderColor(for edge: NSRectEdge) -> NSColor?
```

## Parameters 

`edge`  

The edge of the text block in question.

## Return Value

The border color of the text block edge `edge`.

## See Also

### Working with color

var backgroundColor: NSColor?

The background color of the text block.

func setBorderColor(NSColor?, for: NSRectEdge)

Sets the border color of the specified edge of the text block.

func setBorderColor(NSColor?)

Sets the color of all borders of the text block.

