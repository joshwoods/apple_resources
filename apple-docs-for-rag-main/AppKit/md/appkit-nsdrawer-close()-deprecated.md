

- AppKit
- NSDrawer
-  close() Deprecated

Instance Method

# close()

If the receiver is open, this method closes it.

macOS 10.0–10.13Deprecated

``` source
@MainActor
func close()
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Discussion

Calling `close` on a closed drawer does nothing. You can get the state of a drawer by sending it state.

## See Also

### Opening and Closing Drawers

func close(Any?)

An action method to close the receiver.

Deprecated

func open()

If the receiver is closed, this method opens it.

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

