

- AppKit
- NSDrawerDelegate
-  drawerWillClose(\_:) Deprecated

Instance Method

# drawerWillClose(\_:)

Notifies the delegate the drawer will close.

macOS 10.0–10.13Deprecated

``` source
optional func drawerWillClose(_ notification: Notification)
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Parameters 

`notification`  

An NSDrawerDelegate notification sent by the default notification center immediately before the drawer is closed.

## See Also

### Opening and Closing Drawers

func drawerShouldOpen(NSDrawer) -> Bool

Asks the delegate if the specified drawer should open.

Deprecated

func drawerWillOpen(Notification)

Notifies the delegate that the drawer will open.

Deprecated

func drawerDidOpen(Notification)

Notifies the delegate that the drawer has opened.

Deprecated

func drawerShouldClose(NSDrawer) -> Bool

Asks the delegate if the specified drawer should close.

Deprecated

func drawerDidClose(Notification)

Notifies the delegate that the drawer has closed.

Deprecated

