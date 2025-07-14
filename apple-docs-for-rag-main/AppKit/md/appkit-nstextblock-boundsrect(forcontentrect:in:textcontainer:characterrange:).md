

- AppKit
- NSTextBlock
-  boundsRect(forContentRect:in:textContainer:characterRange:) 

Instance Method

# boundsRect(forContentRect:in:textContainer:characterRange:)

Returns the rectangle the text in the block actually occupies, including padding, borders, and margins.

macOS

``` source
func boundsRect(
    forContentRect contentRect: NSRect,
    in rect: NSRect,
    textContainer: NSTextContainer,
    characterRange charRange: NSRange
) -> NSRect
```

## Parameters 

`contentRect`  

The actual rectangle in which the text was laid out, as determined by rectForLayout(at:in:textContainer:characterRange:).

`rect`  

The initial rectangle in `textContainer` proposed by the typesetter.

`textContainer`  

The text container being used for the layout.

`charRange`  

The range of the characters in the NSTextStorage object whose glyphs are to be drawn.

## Return Value

The rectangle the text in the block actually occupies, including padding, borders, and margins.

## Discussion

This methods is called by the typesetter after the text block is laid out to return the rectangle the text in the block actually occupies, including padding, borders, and margins.

## See Also

### Determining size and position of a text block

func rectForLayout(at: NSPoint, in: NSRect, textContainer: NSTextContainer, characterRange: NSRange) -> NSRect

Returns the rectangle within which glyphs should be laid out for the specified arguments.

