

- AppKit
- NSView
-  menu(for:) 

Instance Method

# menu(for:)

Overridden by subclasses to return a context-sensitive pop-up menu for a given mouse-down event.

macOS

``` source
@MainActor
func menu(for event: NSEvent) -> NSMenu?
```

## Parameters 

`event`  

An object representing a mouse-down event.

## Mentioned in 

Supporting Writing Tools via the pasteboard

## Discussion

The view can use information in the mouse event, such as its location over a particular element of the view, to determine what kind of menu to return. For example, a text object might display a text-editing menu when the cursor lies over text and a menu for changing graphics attributes when the cursor lies over an embedded image.

The default implementation returns the view’s normal menu.

## See Also

### Related Documentation

var menu: NSMenu?

Returns the responder’s menu.

### Managing Contextual Menus

class var defaultMenu: NSMenu?

Overridden by subclasses to return the default pop-up menu for instances of the receiving class.

func willOpenMenu(NSMenu, with: NSEvent)

Called just before a contextual menu for a view is opened on screen.

func didCloseMenu(NSMenu, with: NSEvent?)

Called after a contextual menu that was displayed from the receiving view has been closed.

