

- AppKit
- NSDrawer
-  open(\_:) Deprecated

Instance Method

# open(\_:)

An action method to open the drawer.

macOS 10.0–10.13Deprecated

``` source
@MainActor
func open(_ sender: Any?)
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Parameters 

`sender`  

A user interface element, such as a button or menu item, that invokes the action method.

## Discussion

This method is an action method and likely would not be invoked programatically. Rather, it is an action that is commonly connected in Interface Builder.

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

func open(on: NSRectEdge)

Causes the receiver to open on the specified edge of the parent window.

Deprecated

func toggle(Any?)

Toggles the drawer open or closed.

Deprecated

var state: Int

The state of the receiver.

Deprecated

