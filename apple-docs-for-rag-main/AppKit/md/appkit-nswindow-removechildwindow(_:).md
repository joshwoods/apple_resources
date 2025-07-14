

- AppKit
- NSWindow
-  removeChildWindow(\_:) 

Instance Method

# removeChildWindow(\_:)

Detaches a given child window from the window.

macOS

``` source
@MainActor
func removeChildWindow(_ childWin: NSWindow)
```

## Parameters 

`childWin`  

The child window to detach.

## See Also

### Managing Attached Windows

var childWindows: [NSWindow]?

An array of the window’s attached child windows.

func addChildWindow(NSWindow, ordered: NSWindow.OrderingMode)

Adds a given window as a child window of the window.

var parent: NSWindow?

The parent window to which the window is attached as a child.

