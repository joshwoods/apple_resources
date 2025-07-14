

- AppKit
-  NSDrawerDelegate Deprecated

Protocol

# NSDrawerDelegate

A set of methods that drawer delegates implement to open, close, and resize the drawer.

macOS

``` source
protocol NSDrawerDelegate : NSObjectProtocol
```

Deprecated

Drawers are deprecated and should not be used in modern macOS apps.

## Topics

### Opening and Closing Drawers

func drawerShouldOpen(NSDrawer) -> Bool

Asks the delegate if the specified drawer should open.

func drawerWillOpen(Notification)

Notifies the delegate that the drawer will open.

func drawerDidOpen(Notification)

Notifies the delegate that the drawer has opened.

func drawerShouldClose(NSDrawer) -> Bool

Asks the delegate if the specified drawer should close.

func drawerWillClose(Notification)

Notifies the delegate the drawer will close.

func drawerDidClose(Notification)

Notifies the delegate that the drawer has closed.

### Managing Drawer Size

func drawerWillResizeContents(NSDrawer, to: NSSize) -> NSSize

Invoked when the user resizes the drawer or parent.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Protocols

NSAccessibility

A legacy, informal protocol that Apple doesn’t recommend for active use.

NSEditor

A set of methods that controllers and UI elements can implement to manage editing.

protocol NSEditorRegistration

A set of methods that controllers can implement to enable an editor view to inform the controller when it has uncommitted changes.

protocol NSInputServiceProvider

protocol NSInputServerMouseTracker

