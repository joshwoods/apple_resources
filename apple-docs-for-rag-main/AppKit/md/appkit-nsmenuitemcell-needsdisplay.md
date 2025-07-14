

- AppKit
- NSMenuItemCell
-  needsDisplay 

Instance Property

# needsDisplay

A Boolean value indicating whether the menu item needs to be displayed.

macOS

``` source
@MainActor
var needsDisplay: Bool { get set }
```

## Discussion

Set this property to true when you want the menu item to be drawn.

## See Also

### Drawing the Menu Item

func drawBorderAndBackground(withFrame: NSRect, in: NSView)

Draws the borders and background associated with the receiver’s menu item (if any).

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

