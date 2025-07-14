

- AppKit
- NSMenu
-  popUpContextMenu(\_:with:for:with:) 

Type Method

# popUpContextMenu(\_:with:for:with:)

Displays a contextual menu over a view for an event using a specified font.

macOS

``` source
class func popUpContextMenu(
    _ menu: NSMenu,
    with event: NSEvent,
    for view: NSView,
    with font: NSFont?
)
```

## Parameters 

`menu`  

The menu object to use for the contextual menu.

`event`  

An NSEvent object representing the event.

`view`  

The view object over which to display the contextual menu.

`font`  

An NSFont object representing the font for the contextual menu. If you pass in `nil` for the font, the method uses the default font for `menu`.

## Discussion

Specifying a font using the font parameter is discouraged. Instead, set the menu’s font using the font property, then pass `nil` for the `font` parameter.

## See Also

### Displaying Context-Sensitive Help

class func popUpContextMenu(NSMenu, with: NSEvent, for: NSView)

Displays a contextual menu over a view for an event.

func helpRequested(with: NSEvent)

Overridden by subclasses to implement specialized context-sensitive help behavior.

Deprecated

func popUp(positioning: NSMenuItem?, at: NSPoint, in: NSView?) -> Bool

Pops up the menu at the specified location.

