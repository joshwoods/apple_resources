

- AppKit
- NSTextBlock
-  drawBackground(withFrame:in:characterRange:layoutManager:) 

Instance Method

# drawBackground(withFrame:in:characterRange:layoutManager:)

Called by the layout manager to draw any colors and other decorations before the text is drawn.

macOS

``` source
func drawBackground(
    withFrame frameRect: NSRect,
    in controlView: NSView,
    characterRange charRange: NSRange,
    layoutManager: NSLayoutManager
)
```

## Parameters 

`frameRect`  

The bounds rectangle in view coordinates.

`controlView`  

The view in which drawing occurs.

`charRange`  

The range of the characters in the NSTextStorage object whose glyphs are to be drawn.

`layoutManager`  

The layout manager controlling the typesetting.

