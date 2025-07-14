

- AppKit
- NSCell
-  defaultMenu 

Type Property

# defaultMenu

Returns the default menu for instances of the cell.

macOS

``` source
@MainActor
class var defaultMenu: NSMenu? { get }
```

## Return Value

The default menu. The `NSCell` implementation of this method returns `nil`.

## See Also

### Managing Menus

var menu: NSMenu?

The cell’s contextual menu.

func menu(for: NSEvent, in: NSRect, of: NSView) -> NSMenu?

Returns the menu associated with the cell and related to the specified event and frame.

