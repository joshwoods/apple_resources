

- AppKit
- NSResponder
-  menu 

Instance Property

# menu

Returns the responder’s menu.

macOS

``` source
@MainActor
var menu: NSMenu? { get set }
```

## Discussion

For `NSApplication` this menu is the same as the menu returned by its mainMenu property.

## See Also

### Related Documentation

class var defaultMenu: NSMenu?

Overridden by subclasses to return the default pop-up menu for instances of the receiving class.

func menu(for: NSEvent) -> NSMenu?

Overridden by subclasses to return a context-sensitive pop-up menu for a given mouse-down event.

