

- AppKit
- NSMenuItemCell
-  drawImage(withFrame:in:) 

Instance Method

# drawImage(withFrame:in:)

Draws the image associated with the menu item.

macOS

``` source
@MainActor
func drawImage(
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

This method invokes the `NSCell` method imageRect(forBounds:), passing it `cellFrame`, to calculate the rectangle in which to draw the image. This method is invoked by the cell’s `drawWithFrame:` method. You should not need to invoke it directly. Subclasses may override this method to control the drawing of the image.

## See Also

### Drawing the Menu Item

func drawBorderAndBackground(withFrame: NSRect, in: NSView)

Draws the borders and background associated with the receiver’s menu item (if any).

func drawKeyEquivalent(withFrame: NSRect, in: NSView)

Draws the key equivalent associated with the menu item.

func drawSeparatorItem(withFrame: NSRect, in: NSView)

Draws a menu item separator.

func drawStateImage(withFrame: NSRect, in: NSView)

Draws the state image associated with the menu item.

func drawTitle(withFrame: NSRect, in: NSView)

Draws the title associated with the menu item.

var needsDisplay: Bool

A Boolean value indicating whether the menu item needs to be displayed.

