

- AppKit
- NSView
-  willOpenMenu(\_:with:) 

Instance Method

# willOpenMenu(\_:with:)

Called just before a contextual menu for a view is opened on screen.

macOS 10.11+

``` source
@MainActor
func willOpenMenu(
    _ menu: NSMenu,
    with event: NSEvent
)
```

## Parameters 

`menu`  

The menu that will be opened.

`event`  

The event that caused the menu to open.

## Discussion

This method is called just before a contextual menu for a view is opened on screen. It provides an opportunity to make any desired changes to the visual state of the view. For example, a table view might select a row in response to the contextual menu being displayed.

## See Also

### Managing Contextual Menus

func menu(for: NSEvent) -> NSMenu?

Overridden by subclasses to return a context-sensitive pop-up menu for a given mouse-down event.

class var defaultMenu: NSMenu?

Overridden by subclasses to return the default pop-up menu for instances of the receiving class.

func didCloseMenu(NSMenu, with: NSEvent?)

Called after a contextual menu that was displayed from the receiving view has been closed.

