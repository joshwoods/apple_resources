

- AppKit
- NSCell
-  menu 

Instance Property

# menu

The cell’s contextual menu.

macOS

``` source
@MainActor
var menu: NSMenu? { get set }
```

## Discussion

Use this property to specify a menu containing contextual commands associated with the cell. If the cell does not have a menu, set this property to `nil`.

## See Also

### Managing Menus

class var defaultMenu: NSMenu?

Returns the default menu for instances of the cell.

func menu(for: NSEvent, in: NSRect, of: NSView) -> NSMenu?

Returns the menu associated with the cell and related to the specified event and frame.

