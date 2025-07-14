

- AppKit
- NSView
-  didCloseMenu(\_:with:) 

Instance Method

# didCloseMenu(\_:with:)

Called after a contextual menu that was displayed from the receiving view has been closed.

macOS 10.11+

``` source
@MainActor
func didCloseMenu(
    _ menu: NSMenu,
    with event: NSEvent?
)
```

## Parameters 

`menu`  

The menu that was closed.

`event`  

The event that caused the menu to close, if there was one. If an event did not cause the menu to close, this value is `nil`.

## Discussion

This method is called only if the contextual menu had been opened and the view has previously received the willOpenMenu(_:with:) method. When the view receives didCloseMenu(_:with:), it should reset its visual state, if necessary. For example, if a table view selected a row in response to a contextual menu being displayed, this method could deselect the row.

## See Also

### Managing Contextual Menus

func menu(for: NSEvent) -> NSMenu?

Overridden by subclasses to return a context-sensitive pop-up menu for a given mouse-down event.

class var defaultMenu: NSMenu?

Overridden by subclasses to return the default pop-up menu for instances of the receiving class.

func willOpenMenu(NSMenu, with: NSEvent)

Called just before a contextual menu for a view is opened on screen.

