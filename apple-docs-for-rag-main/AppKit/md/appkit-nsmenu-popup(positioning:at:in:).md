

- AppKit
- NSMenu
-  popUp(positioning:at:in:) 

Instance Method

# popUp(positioning:at:in:)

Pops up the menu at the specified location.

macOS 10.6+

``` source
func popUp(
    positioning item: NSMenuItem?,
    at location: NSPoint,
    in view: NSView?
) -> Bool
```

## Parameters 

`item`  

The menu item to be positioned at the specified location in the view.

`location`  

The location in the `view` coordinate system to display the menu item.

`view`  

The view to display the menu item over.

## Return Value

true if menu tracking ended because an item was selected, and false if menu tracking was cancelled for any reason.

## Discussion

Displays the menu as a pop-up menu. The top left corner of the specified item (if specified, `item` must be present in the menu) is positioned at the specified location in the specified view, interpreted in the view’s own coordinate system.

If `item` is `nil`, the menu is positioned such that the top left of the menu content frame is at the given location.

If `view` is `nil`, the location is interpreted in the screen coordinate system. This allows you to pop up a menu disconnected from any window.

## See Also

### Displaying Context-Sensitive Help

class func popUpContextMenu(NSMenu, with: NSEvent, for: NSView)

Displays a contextual menu over a view for an event.

class func popUpContextMenu(NSMenu, with: NSEvent, for: NSView, with: NSFont?)

Displays a contextual menu over a view for an event using a specified font.

func helpRequested(with: NSEvent)

Overridden by subclasses to implement specialized context-sensitive help behavior.

Deprecated

