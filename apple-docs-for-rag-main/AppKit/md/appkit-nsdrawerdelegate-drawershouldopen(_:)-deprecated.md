

- AppKit
- NSDrawerDelegate
-  drawerShouldOpen(\_:) Deprecated

Instance Method

# drawerShouldOpen(\_:)

Asks the delegate if the specified drawer should open.

macOS 10.0–10.13Deprecated

``` source
optional func drawerShouldOpen(_ sender: NSDrawer) -> Bool
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Parameters 

`sender`  

The drawer requesting permission to open.

## Return Value

true if the drawer should open; false to prevent the drawer from opening.

## Discussion

This method is invoked on user-initiated attempts to open a drawer by dragging it or when the NSDrawerDelegate method is called.

## See Also

### Related Documentation

Drawer Programming Topics

### Opening and Closing Drawers

func drawerWillOpen(Notification)

Notifies the delegate that the drawer will open.

Deprecated

func drawerDidOpen(Notification)

Notifies the delegate that the drawer has opened.

Deprecated

func drawerShouldClose(NSDrawer) -> Bool

Asks the delegate if the specified drawer should close.

Deprecated

func drawerWillClose(Notification)

Notifies the delegate the drawer will close.

Deprecated

func drawerDidClose(Notification)

Notifies the delegate that the drawer has closed.

Deprecated

