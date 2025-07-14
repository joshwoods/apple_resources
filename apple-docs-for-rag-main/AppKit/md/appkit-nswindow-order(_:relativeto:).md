

- AppKit
- NSWindow
-  order(\_:relativeTo:) 

Instance Method

# order(\_:relativeTo:)

Repositions the window’s window device in the window server’s screen list.

macOS

``` source
@MainActor
func order(
    _ place: NSWindow.OrderingMode,
    relativeTo otherWin: Int
)
```

## Parameters 

`place`  

\- NSWindow.OrderingMode.out: The window is removed from the screen list and `otherWin` is ignored.

- NSWindow.OrderingMode.above: The window is ordered immediately in front of the window whose window number is `otherWin`

- NSWindow.OrderingMode.below: The window is placed immediately behind the window represented by `otherWin`.

`otherWin`  

The number of the window the window is to be placed in front of or behind. Pass `0` to place the window in front of (when `place` is `NSWindowAbove`) or behind (when `place` is `NSWindowBelow`) all other windows in its level.

## See Also

### Related Documentation

var windowNumber: Int

The window number of the window’s window device.

func makeKeyAndOrderFront(Any?)

Moves the window to the front of the screen list, within its level, and makes it the key window; that is, it shows the window.

### Managing Window Layers

func orderOut(Any?)

Removes the window from the screen list, which hides the window.

func orderBack(Any?)

Moves the window to the back of its level in the screen list, without changing either the key window or the main window.

func orderFront(Any?)

Moves the window to the front of its level in the screen list, without changing either the key window or the main window.

func orderFrontRegardless()

Moves the window to the front of its level, even if its application isn’t active, without changing either the key window or the main window.

var level: NSWindow.Level

The window level of the window.

struct Level

The standard window levels in macOS.

