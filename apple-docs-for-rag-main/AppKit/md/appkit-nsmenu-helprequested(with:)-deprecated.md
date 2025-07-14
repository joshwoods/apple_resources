

- AppKit
- NSMenu
-  helpRequested(with:) Deprecated

Instance Method

# helpRequested(with:)

Overridden by subclasses to implement specialized context-sensitive help behavior.

macOS 10.0–10.11Deprecated

``` source
func helpRequested(with eventPtr: NSEvent)
```

## Parameters 

`eventPtr`  

An NSEvent object representing the event associated with the help request.

## Discussion

Subclasses in their implementation of this method should cause the Help Manager (NSHelpManager) to display the help associated with the menu. Never invoke this method directly.

### Special Considerations

In macOS 10.6 and later this method has no effect. This method may be deprecated in a future release.

## See Also

### Related Documentation

func showContextHelp(for: Any, locationHint: NSPoint) -> Bool

Displays the context-sensitive help for a given object at or near the point on the screen specified by a given point.

### Displaying Context-Sensitive Help

class func popUpContextMenu(NSMenu, with: NSEvent, for: NSView)

Displays a contextual menu over a view for an event.

class func popUpContextMenu(NSMenu, with: NSEvent, for: NSView, with: NSFont?)

Displays a contextual menu over a view for an event using a specified font.

func popUp(positioning: NSMenuItem?, at: NSPoint, in: NSView?) -> Bool

Pops up the menu at the specified location.

