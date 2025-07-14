

- AppKit
- NSApplication
-  makeWindowsPerform(\_:inOrder:) Deprecated

Instance Method

# makeWindowsPerform(\_:inOrder:)

Sends the specified message to each of the app’s window objects until one returns a non-`nil` value.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func makeWindowsPerform(
    _ selector: Selector,
    inOrder: Bool
) -> NSWindow?
```

Deprecated

Use enumerateWindows(options:using:) instead.

## Parameters 

`selector`  

The selector to perform on each window. This method must not take any arguments and must return a value whose type that can be compared to `nil`.

`inOrder`  

If true, the `aSelector` message is sent to each of the window server’s onscreen windows, going in z-order, until one returns a non-`nil` value. A minimized window is not considered to be onscreen for this check. If false, the message is sent to all windows in `NSApp`’s window list, regardless of whether or not they are onscreen. This order is unspecified.

## Return Value

The window that returned a non-`nil` value or `nil` if all windows returned nil from `aSelector`.

## See Also

### Related Documentation

func tryToPerform(Selector, with: Any?) -> Bool

Dispatches an action message to the specified target.

func sendAction(Selector, to: Any?, from: Any?) -> Bool

Sends the given action message to the given target.

### Managing App Windows

var keyWindow: NSWindow?

The window that currently receives keyboard events.

var mainWindow: NSWindow?

The app’s main window.

func window(withWindowNumber: Int) -> NSWindow?

Returns the window corresponding to the specified window number.

var windows: [NSWindow]

An array of the app’s window objects.

func enumerateWindows(options: NSApplication.WindowListOptions, using: (NSWindow, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a block for each of the app’s windows.

struct WindowListOptions

This constant indicates a window ordering.

