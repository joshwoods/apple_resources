

- AppKit
- NSWindow
-  childWindows 

Instance Property

# childWindows

An array of the window’s attached child windows.

macOS

``` source
@MainActor
var childWindows: [NSWindow]? { get }
```

## See Also

### Managing Attached Windows

func addChildWindow(NSWindow, ordered: NSWindow.OrderingMode)

Adds a given window as a child window of the window.

func removeChildWindow(NSWindow)

Detaches a given child window from the window.

var parent: NSWindow?

The parent window to which the window is attached as a child.

