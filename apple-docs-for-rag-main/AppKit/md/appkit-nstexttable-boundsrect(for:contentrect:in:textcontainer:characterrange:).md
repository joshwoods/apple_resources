

- AppKit
- NSTextTable
-  boundsRect(for:contentRect:in:textContainer:characterRange:) 

Instance Method

# boundsRect(for:contentRect:in:textContainer:characterRange:)

Returns the rectangle the text table block actually occupies, including padding, borders, and margins.

macOS

``` source
func boundsRect(
    for block: NSTextTableBlock,
    contentRect: NSRect,
    in rect: NSRect,
    textContainer: NSTextContainer,
    characterRange charRange: NSRange
) -> NSRect
```

## Parameters 

`block`  

The text table block that wants to determine where to layout its glyphs.

`contentRect`  

The actual rectangle in which the text was laid out, as determined by rectForLayout(at:in:textContainer:characterRange:).

`rect`  

The initial rectangle in `textContainer` proposed by the typesetter.

`textContainer`  

The text container being used for the layout.

`charRange`  

The range of the characters whose glyphs are to be drawn.

## Return Value

The rectangle the text table block actually occupies, including padding, borders, and margins.

## Discussion

This method is called by the text table block `block` after it is laid out to determine the rectangle the text table block actually occupies, including padding, borders, and margins.

## See Also

### Determining layout rectangles

func rect(for: NSTextTableBlock, layoutAt: NSPoint, in: NSRect, textContainer: NSTextContainer, characterRange: NSRange) -> NSRect

Returns the rectangle within which glyphs should be laid out for a text table block.

