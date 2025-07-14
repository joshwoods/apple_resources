

- AppKit
- NSMenu
-  popUpContextMenu(\_:with:for:) 

Type Method

# popUpContextMenu(\_:with:for:)

Displays a contextual menu over a view for an event.

macOS

``` source
class func popUpContextMenu(
    _ menu: NSMenu,
    with event: NSEvent,
    for view: NSView
)
```

## Parameters 

`menu`  

The menu object to use for the contextual menu.

`event`  

An NSEvent object representing the event.

`view`  

The view object over which to display the contextual menu.

## Mentioned in 

Supporting Continuity Camera in Your Mac App

Supporting Writing Tools via the pasteboard

## See Also

### Displaying Context-Sensitive Help

class func popUpContextMenu(NSMenu, with: NSEvent, for: NSView, with: NSFont?)

Displays a contextual menu over a view for an event using a specified font.

func helpRequested(with: NSEvent)

Overridden by subclasses to implement specialized context-sensitive help behavior.

Deprecated

func popUp(positioning: NSMenuItem?, at: NSPoint, in: NSView?) -> Bool

Pops up the menu at the specified location.

