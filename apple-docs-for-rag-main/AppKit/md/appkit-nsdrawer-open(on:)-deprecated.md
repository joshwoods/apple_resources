

- AppKit
- NSDrawer
-  open(on:) Deprecated

Instance Method

# open(on:)

Causes the receiver to open on the specified edge of the parent window.

macOS 10.0–10.13Deprecated

``` source
@MainActor
func open(on edge: NSRectEdge)
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Parameters 

`edge`  

The edge of the parent window on which to open the receiver. See Constants for a list of edge constants and locations.

## See Also

### Opening and Closing Drawers

func close()

If the receiver is open, this method closes it.

Deprecated

func close(Any?)

An action method to close the receiver.

Deprecated

func open()

If the receiver is closed, this method opens it.

Deprecated

func open(Any?)

An action method to open the drawer.

Deprecated

func toggle(Any?)

Toggles the drawer open or closed.

Deprecated

var state: Int

The state of the receiver.

Deprecated

