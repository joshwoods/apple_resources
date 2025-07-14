

- AppKit
- NSTextTable
-  rect(for:layoutAt:in:textContainer:characterRange:) 

Instance Method

# rect(for:layoutAt:in:textContainer:characterRange:)

Returns the rectangle within which glyphs should be laid out for a text table block.

macOS

``` source
func rect(
    for block: NSTextTableBlock,
    layoutAt startingPoint: NSPoint,
    in rect: NSRect,
    textContainer: NSTextContainer,
    characterRange charRange: NSRange
) -> NSRect
```

## Parameters 

`block`  

The text table block that wants to determine where to layout its glyphs.

`startingPoint`  

The location, in container coordinates, where layout begins.

`rect`  

The rectangle in which the block is constrained to lie. For top-level blocks, this is the container rectangle of `textContainer`; for nested blocks, this is the layout rectangle of the enclosing block.

`textContainer`  

The text container being used for the layout.

`charRange`  

The range of the characters whose glyphs are to be drawn.

## Return Value

The rectangle within which glyphs should be laid out.

## Discussion

This method is called by the text table block `block` to determine the rectangle within which glyphs should be laid out for the text table block.

## See Also

### Determining layout rectangles

func boundsRect(for: NSTextTableBlock, contentRect: NSRect, in: NSRect, textContainer: NSTextContainer, characterRange: NSRange) -> NSRect

Returns the rectangle the text table block actually occupies, including padding, borders, and margins.

