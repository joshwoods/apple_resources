

- AppKit
- NSWindow
-  makeKeyAndOrderFront(\_:) 

Instance Method

# makeKeyAndOrderFront(\_:)

Moves the window to the front of the screen list, within its level, and makes it the key window; that is, it shows the window.

macOS

``` source
@MainActor
func makeKeyAndOrderFront(_ sender: Any?)
```

## Parameters 

`sender`  

The message’s sender.

## See Also

### Related Documentation

func orderBack(Any?)

Moves the window to the back of its level in the screen list, without changing either the key window or the main window.

func orderFront(Any?)

Moves the window to the front of its level in the screen list, without changing either the key window or the main window.

var level: NSWindow.Level

The window level of the window.

func order(NSWindow.OrderingMode, relativeTo: Int)

Repositions the window’s window device in the window server’s screen list.

func orderOut(Any?)

Removes the window from the screen list, which hides the window.

### Managing Key Status

var isKeyWindow: Bool

A Boolean value that indicates whether the window is the key window for the application.

var canBecomeKey: Bool

A Boolean value that indicates whether the window can become the key window.

func makeKey()

Makes the window the key window.

func becomeKey()

Informs the window that it has become the key window.

func resignKey()

Resigns the window’s key window status.

