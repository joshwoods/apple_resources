

- AppKit
- NSWindow
-  orderFrontRegardless() 

Instance Method

# orderFrontRegardless()

Moves the window to the front of its level, even if its application isn’t active, without changing either the key window or the main window.

macOS

``` source
@MainActor
func orderFrontRegardless()
```

## Discussion

Normally an `NSWindow` object can’t be moved in front of the key window unless it and the key window are in the same application. You should rarely need to invoke this method; it’s designed to be used when applications are cooperating in such a way that an active application (with the key window) is using another application to display data.

## See Also

### Managing Window Layers

func orderOut(Any?)

Removes the window from the screen list, which hides the window.

func orderBack(Any?)

Moves the window to the back of its level in the screen list, without changing either the key window or the main window.

func orderFront(Any?)

Moves the window to the front of its level in the screen list, without changing either the key window or the main window.

func order(NSWindow.OrderingMode, relativeTo: Int)

Repositions the window’s window device in the window server’s screen list.

var level: NSWindow.Level

The window level of the window.

struct Level

The standard window levels in macOS.

