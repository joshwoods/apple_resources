

- AppKit
- NSCell
-  menu(for:in:of:) 

Instance Method

# menu(for:in:of:)

Returns the menu associated with the cell and related to the specified event and frame.

macOS

``` source
@MainActor
func menu(
    for event: NSEvent,
    in cellFrame: NSRect,
    of view: NSView
) -> NSMenu?
```

## Parameters 

`event`  

The event used to find the menu.

`cellFrame`  

The cell’s rectangle. This rectangle indicates the region containing the cursor.

`view`  

The view that manages the cell. This is usually the control object that owns the cell.

## Return Value

The menu associated with the cell and event parameters, or `nil` if no menu is set.

## Discussion

This method is usually invoked by the NSControl object (`aView`) managing the receiver. The default implementation gets the value of the menu property and returns `nil` if no menu has been set. Subclasses can override to customize the returned menu according to the event received and the area in which the mouse event occurs.

## See Also

### Managing Menus

class var defaultMenu: NSMenu?

Returns the default menu for instances of the cell.

var menu: NSMenu?

The cell’s contextual menu.

