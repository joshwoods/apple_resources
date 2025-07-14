

- AppKit
- NSDrawer
-  toggle(\_:) Deprecated

Instance Method

# toggle(\_:)

Toggles the drawer open or closed.

macOS 10.0–10.13Deprecated

``` source
@MainActor
func toggle(_ sender: Any?)
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Parameters 

`sender`  

The sender of the message.

## Discussion

If the receiver is closed, or in the process of either opening or closing, it is opened. Otherwise, the drawer is closed.

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

func open(on: NSRectEdge)

Causes the receiver to open on the specified edge of the parent window.

Deprecated

var state: Int

The state of the receiver.

Deprecated

