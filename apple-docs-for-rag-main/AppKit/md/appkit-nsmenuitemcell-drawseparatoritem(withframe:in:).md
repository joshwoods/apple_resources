

- AppKit
- NSMenuItemCell
-  drawSeparatorItem(withFrame:in:) 

Instance Method

# drawSeparatorItem(withFrame:in:)

Draws a menu item separator.

macOS

``` source
@MainActor
func drawSeparatorItem(
    withFrame cellFrame: NSRect,
    in controlView: NSView
)
```

## Parameters 

`cellFrame`  

A rectangle defining the receiver’s frame area.

`controlView`  

The view object that contains this cell (usually an NSControl object).

## Discussion

This method uses the `cellFrame` parameter to calculate the rectangle in which to draw the menu item separator. This method uses the `controlView` to determine whether the separator item should be drawn normally or flipped.

You should not need to invoke this method directly. Subclasses may override this method to control the drawing of the separator.

## See Also

### Related Documentation

var isFlipped: Bool

A Boolean value indicating whether the view uses a flipped coordinate system.

### Drawing the Menu Item

func drawBorderAndBackground(withFrame: NSRect, in: NSView)

Draws the borders and background associated with the receiver’s menu item (if any).

func drawImage(withFrame: NSRect, in: NSView)

Draws the image associated with the menu item.

func drawKeyEquivalent(withFrame: NSRect, in: NSView)

Draws the key equivalent associated with the menu item.

func drawStateImage(withFrame: NSRect, in: NSView)

Draws the state image associated with the menu item.

func drawTitle(withFrame: NSRect, in: NSView)

Draws the title associated with the menu item.

var needsDisplay: Bool

A Boolean value indicating whether the menu item needs to be displayed.

