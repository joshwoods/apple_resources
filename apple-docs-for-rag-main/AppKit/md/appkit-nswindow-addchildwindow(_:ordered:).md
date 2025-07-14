

- AppKit
- NSWindow
-  addChildWindow(\_:ordered:) 

Instance Method

# addChildWindow(\_:ordered:)

Adds a given window as a child window of the window.

macOS

``` source
@MainActor
func addChildWindow(
    _ childWin: NSWindow,
    ordered place: NSWindow.OrderingMode
)
```

## Parameters 

`childWin`  

The child window to order.

`place`  

\- NSWindow.OrderingMode.above: `childWin` is ordered immediately in front of the window.

- NSWindow.OrderingMode.below: `childWin` is ordered immediately behind the window.

## Discussion

After the `childWin` is added as a child of the window, it is maintained in relative position indicated by `place` for subsequent ordering operations involving either window. While this attachment is active, moving `childWin` will not cause the window to move (as in sliding a drawer in or out), but moving the window will cause `childWin` to move.

Note that you should not create cycles between parent and child windows. For example, you should not add window B as child of window A, then add window A as a child of window B.

## See Also

### Managing Attached Windows

var childWindows: [NSWindow]?

An array of the window’s attached child windows.

func removeChildWindow(NSWindow)

Detaches a given child window from the window.

var parent: NSWindow?

The parent window to which the window is attached as a child.

