

- AppKit
- NSPopUpButton
-  pullsDown 

Instance Property

# pullsDown

A Boolean value indicating whether the button displays a pull-down or pop-up menu.

macOS

``` source
@MainActor
var pullsDown: Bool { get set }
```

## Discussion

When the value of this property is true, the button displays a pull-down menu; otherwise, it displays a pop-up menu. This property does not affect the contents of the menu; it affects only the style of the menu.

When changing the menu type to a pull-down menu, if the menu was a pop-up menu and the cell alters the state of its selected items, this method sets the state of the currently selected item to `NSStateOff` before changing the menu type.

## See Also

### Related Documentation

init(frame: NSRect, pullsDown: Bool)

Returns an `NSPopUpButton` object initialized to the specified dimensions.

### Setting the type of menu

var autoenablesItems: Bool

A Boolean value indicating whether the button enables and disables its items every time a user event occurs.

