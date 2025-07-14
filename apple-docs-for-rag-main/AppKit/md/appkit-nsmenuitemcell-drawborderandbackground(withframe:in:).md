

- AppKit
- NSMenuItemCell
-  drawBorderAndBackground(withFrame:in:) 

Instance Method

# drawBorderAndBackground(withFrame:in:)

Draws the borders and background associated with the receiver’s menu item (if any).

macOS

``` source
@MainActor
func drawBorderAndBackground(
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

This method invokes the `NSCell` method imageRect(forBounds:), passing it `cellFrame`, to calculate the rectangle in which to draw the image. The cell invokes this method before invoking the methods to draw the other menu item components.

## See Also

### Related Documentation

func draw(withFrame: NSRect, in: NSView)

Draws the receiver’s border and then draws the interior of the cell.

### Drawing the Menu Item

func drawImage(withFrame: NSRect, in: NSView)

Draws the image associated with the menu item.

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

