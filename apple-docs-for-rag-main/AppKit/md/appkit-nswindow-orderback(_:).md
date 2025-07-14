

- AppKit
- NSWindow
-  orderBack(\_:) 

Instance Method

# orderBack(\_:)

Moves the window to the back of its level in the screen list, without changing either the key window or the main window.

macOS

``` source
@MainActor
func orderBack(_ sender: Any?)
```

## Parameters 

`sender`  

Message originator.

## See Also

### Related Documentation

func makeKeyAndOrderFront(Any?)

Moves the window to the front of the screen list, within its level, and makes it the key window; that is, it shows the window.

### Managing Window Layers

func orderOut(Any?)

Removes the window from the screen list, which hides the window.

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

