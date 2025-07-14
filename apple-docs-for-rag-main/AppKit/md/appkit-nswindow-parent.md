

- AppKit
- NSWindow
-  parent 

Instance Property

# parent

The parent window to which the window is attached as a child.

macOS

``` source
@MainActor
weak var parent: NSWindow? { get set }
```

## Discussion

This property should be set from a subclass when it is overridden by a subclass’s implementation. It should not be set otherwise.

Note that calling orderOut(_:) on a child window causes the window to be removed from its parent window before it is itself removed.

## See Also

### Managing Attached Windows

var childWindows: [NSWindow]?

An array of the window’s attached child windows.

func addChildWindow(NSWindow, ordered: NSWindow.OrderingMode)

Adds a given window as a child window of the window.

func removeChildWindow(NSWindow)

Detaches a given child window from the window.

