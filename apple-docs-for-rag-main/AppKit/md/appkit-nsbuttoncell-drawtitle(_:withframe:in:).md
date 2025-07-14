

- AppKit
- NSButtonCell
-  drawTitle(\_:withFrame:in:) 

Instance Method

# drawTitle(\_:withFrame:in:)

Draws the button’s title centered vertically in a specified rectangle.

macOS

``` source
@MainActor
func drawTitle(
    _ title: NSAttributedString,
    withFrame frame: NSRect,
    in controlView: NSView
) -> NSRect
```

## Parameters 

`title`  

The title of the button.

`frame`  

The rectangle in which to draw the title.

`controlView`  

The control being drawn.

## Return Value

The bounding rectangle for the text of the title.

## Discussion

This method is called automatically when the button is redrawn; you should not call it directly.

## See Also

### Related Documentation

var attributedTitle: NSAttributedString

The title displayed by the button when it’s in its normal state as an attributed string.

var alternateTitle: String

The string displayed by the button when it’s in its alternate state.

### Drawing the Button Content

func drawBezel(withFrame: NSRect, in: NSView)

Draws the border of the button using the current bezel style.

func drawImage(NSImage, withFrame: NSRect, in: NSView)

Draws the image associated with the button’s current state.

