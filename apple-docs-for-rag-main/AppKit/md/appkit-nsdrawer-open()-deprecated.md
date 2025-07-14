

- AppKit
- NSDrawer
-  open() Deprecated

Instance Method

# open()

If the receiver is closed, this method opens it.

macOS 10.0–10.13Deprecated

``` source
@MainActor
func open()
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Discussion

Calling `open` on an open drawer does nothing. You can get the state of a drawer by sending it state. If an edge is not specified, an attempt will be made to choose an edge based on the space available to display the drawer onscreen. If you need to ensure that a drawer opens on a particular edge, use open(on:).

## See Also

### Opening and Closing Drawers

func close()

If the receiver is open, this method closes it.

Deprecated

func close(Any?)

An action method to close the receiver.

Deprecated

func open(Any?)

An action method to open the drawer.

Deprecated

func open(on: NSRectEdge)

Causes the receiver to open on the specified edge of the parent window.

Deprecated

func toggle(Any?)

Toggles the drawer open or closed.

Deprecated

var state: Int

The state of the receiver.

Deprecated

