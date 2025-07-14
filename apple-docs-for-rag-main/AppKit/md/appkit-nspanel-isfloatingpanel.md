

- AppKit
- NSPanel
-  isFloatingPanel 

Instance Property

# isFloatingPanel

A Boolean value that indicates whether the receiver is a floating panel.

macOS

``` source
@MainActor
var isFloatingPanel: Bool { get set }
```

## Discussion

The value of this property is true when the receiver is a floating panel, false otherwise.

By default, panels do not float above other windows. It’s appropriate for a panel to float above other windows only if all of the following conditions are true:

- It’s small enough not to obscure whatever is behind it.

- It’s oriented more to the mouse than to the keyboard—that is, if it doesn’t become the key window or becomes so only when needed.

- It needs to remain visible while the user works in the app’s standard windows—for example, if the user must frequently move the pointer back and forth between a standard window and the panel (such as a tool palette), or if the panel gives information relevant to the user’s actions in a standard window.

- It hides when the app is deactivated (the default behavior for panels).

## See Also

### Related Documentation

var level: NSWindow.Level

The window level of the window.

Window Programming Guide

### Configuring Panels

var becomesKeyOnlyIfNeeded: Bool

A Boolean value that indicates whether the receiver becomes the key window only when needed.

var worksWhenModal: Bool

A Boolean value that indicates whether the panel receives keyboard and mouse events even when some other window is being run modally.

