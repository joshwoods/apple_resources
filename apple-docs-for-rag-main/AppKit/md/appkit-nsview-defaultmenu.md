

- AppKit
- NSView
-  defaultMenu 

Type Property

# defaultMenu

Overridden by subclasses to return the default pop-up menu for instances of the receiving class.

macOS

``` source
@MainActor
class var defaultMenu: NSMenu? { get }
```

## Discussion

The default implementation returns `nil`.

## See Also

### Related Documentation

var menu: NSMenu?

Returns the responder’s menu.

### Managing Contextual Menus

func menu(for: NSEvent) -> NSMenu?

Overridden by subclasses to return a context-sensitive pop-up menu for a given mouse-down event.

func willOpenMenu(NSMenu, with: NSEvent)

Called just before a contextual menu for a view is opened on screen.

func didCloseMenu(NSMenu, with: NSEvent?)

Called after a contextual menu that was displayed from the receiving view has been closed.

