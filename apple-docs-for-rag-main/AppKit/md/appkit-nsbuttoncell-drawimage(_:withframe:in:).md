

- AppKit
- NSButtonCell
-  drawImage(\_:withFrame:in:) 

Instance Method

# drawImage(\_:withFrame:in:)

Draws the image associated with the button’s current state.

macOS

``` source
@MainActor
func drawImage(
    _ image: NSImage,
    withFrame frame: NSRect,
    in controlView: NSView
)
```

## Parameters 

`image`  

The image associated with the button’s current state.

`frame`  

The bounding rectangle of the button.

`controlView`  

The control being drawn.

## Discussion

This method is called automatically when the button is redrawn; you should not call it directly.

You specify the primary and alternate images for the button using Interface Builder.

## See Also

### Related Documentation

var alternateImage: NSImage?

The image the button displays in its alternate state.

### Drawing the Button Content

func drawBezel(withFrame: NSRect, in: NSView)

Draws the border of the button using the current bezel style.

func drawTitle(NSAttributedString, withFrame: NSRect, in: NSView) -> NSRect

Draws the button’s title centered vertically in a specified rectangle.

