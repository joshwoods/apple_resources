

- AppKit
- NSWindow
-  orderOut(\_:) 

Instance Method

# orderOut(\_:)

Removes the window from the screen list, which hides the window.

macOS

``` source
@MainActor
func orderOut(_ sender: Any?)
```

## Parameters 

`sender`  

The window to remove.

## Discussion

If the window is the key or main window, the window object immediately behind it is made key or main in its place. Calling orderOut(_:) causes the window to be removed from the screen, but does not cause it to be released. See the close() method for information on when a window is released. Calling orderOut(_:) on a child window causes the window to be removed from its parent window before being removed.

The default animation based on the window type will be used when the window is ordered out unless it has been modified by the animationBehavior property.

## See Also

### Related Documentation

var isReleasedWhenClosed: Bool

A Boolean value that indicates whether the window is released when it receives the `close` message.

### Managing Window Layers

func orderBack(Any?)

Moves the window to the back of its level in the screen list, without changing either the key window or the main window.

func orderFront(Any?)

Moves the window to the front of its level in the screen list, without changing either the key window or the main window.

func orderFrontRegardless()

Moves the window to the front of its level, even if its application isn’t active, without changing either the key window or the main window.

func order(NSWindow.OrderingMode, relativeTo: Int)

Repositions the window’s window device in the window server’s screen list.

var level: NSWindow.Level

The window level of the window.

struct Level

The standard window levels in macOS.

