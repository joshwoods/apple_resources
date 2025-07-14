

- AppKit
- NSWindow
-  level 

Instance Property

# level

The window level of the window.

macOS

``` source
@MainActor
var level: NSWindow.Level { get set }
```

## Discussion

See `Window Levels` for a list of possible values. Each level in the list groups windows within it in front of those in all preceding groups. Floating windows, for example, appear in front of all normal-level windows.

The constant `NSTornOffMenuWindowLevel` is preferable to its synonym, `NSSubmenuWindowLevel`.

## See Also

### Managing Window Layers

func orderOut(Any?)

Removes the window from the screen list, which hides the window.

func orderBack(Any?)

Moves the window to the back of its level in the screen list, without changing either the key window or the main window.

func orderFront(Any?)

Moves the window to the front of its level in the screen list, without changing either the key window or the main window.

func orderFrontRegardless()

Moves the window to the front of its level, even if its application isn’t active, without changing either the key window or the main window.

func order(NSWindow.OrderingMode, relativeTo: Int)

Repositions the window’s window device in the window server’s screen list.

struct Level

The standard window levels in macOS.

