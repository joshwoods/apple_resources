

- AppKit
- NSButtonCell
-  drawBezel(withFrame:in:) 

Instance Method

# drawBezel(withFrame:in:)

Draws the border of the button using the current bezel style.

macOS

``` source
@MainActor
func drawBezel(
    withFrame frame: NSRect,
    in controlView: NSView
)
```

## Parameters 

`frame`  

The bounding rectangle of the button.

`controlView`  

The control being drawn.

## Discussion

This method is called automatically when the button is redrawn; you should not call it directly.

## See Also

### Related Documentation

var bezelStyle: NSButton.BezelStyle

The appearance of the button’s border, if it has one.

### Drawing the Button Content

func drawImage(NSImage, withFrame: NSRect, in: NSView)

Draws the image associated with the button’s current state.

func drawTitle(NSAttributedString, withFrame: NSRect, in: NSView) -> NSRect

Draws the button’s title centered vertically in a specified rectangle.

