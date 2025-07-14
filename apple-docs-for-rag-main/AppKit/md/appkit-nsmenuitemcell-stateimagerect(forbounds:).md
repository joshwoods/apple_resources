

- AppKit
- NSMenuItemCell
-  stateImageRect(forBounds:) 

Instance Method

# stateImageRect(forBounds:)

Returns the rectangle into which the menu item’s state image should be drawn.

macOS

``` source
@MainActor
func stateImageRect(forBounds cellFrame: NSRect) -> NSRect
```

## Parameters 

`cellFrame`  

A rectangle that defines the bounds of the receiver.

## Return Value

The returned rectangle is based on `cellFrame` but encompasses only the area to be occupied by the menu item’s state image.

## See Also

### Getting the Menu Item’s Drawing Rectangle

func keyEquivalentRect(forBounds: NSRect) -> NSRect

Returns the rectangle into which the menu item’s key equivalent should be drawn.

func titleRect(forBounds: NSRect) -> NSRect

Returns the rectangle into which the menu item’s title should be drawn.

