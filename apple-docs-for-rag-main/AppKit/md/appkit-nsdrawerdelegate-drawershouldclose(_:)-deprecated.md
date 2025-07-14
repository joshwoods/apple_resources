

- AppKit
- NSDrawerDelegate
-  drawerShouldClose(\_:) Deprecated

Instance Method

# drawerShouldClose(\_:)

Asks the delegate if the specified drawer should close.

macOS 10.0–10.13Deprecated

``` source
optional func drawerShouldClose(_ sender: NSDrawer) -> Bool
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Parameters 

`sender`  

The drawer being closed.

## Return Value

true to allow the drawer to close; false to prevent it from closing.

## Discussion

This method is invoked on user-initiated attempts to close a drawer by dragging it or when the NSDrawerDelegate method is called.

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

func drawerWillClose(Notification)

Notifies the delegate the drawer will close.

Deprecated

func drawerDidClose(Notification)

Notifies the delegate that the drawer has closed.

Deprecated

