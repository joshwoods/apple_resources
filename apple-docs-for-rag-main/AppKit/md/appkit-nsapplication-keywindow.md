

- AppKit
- NSApplication
-  keyWindow 

Instance Property

# keyWindow

The window that currently receives keyboard events.

macOS

``` source
@MainActor
weak var keyWindow: NSWindow? { get }
```

## Discussion

The value of this property is `nil` when there is no window receiving keyboard events. The property might be `nil` because the app’s storyboard file has not yet finished loading or when the receiver is not active.

## See Also

### Related Documentation

var isKeyWindow: Bool

A Boolean value that indicates whether the window is the key window for the application.

### Managing App Windows

var mainWindow: NSWindow?

The app’s main window.

func window(withWindowNumber: Int) -> NSWindow?

Returns the window corresponding to the specified window number.

var windows: [NSWindow]

An array of the app’s window objects.

func makeWindowsPerform(Selector, inOrder: Bool) -> NSWindow?

Sends the specified message to each of the app’s window objects until one returns a non-`nil` value.

Deprecated

func enumerateWindows(options: NSApplication.WindowListOptions, using: (NSWindow, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a block for each of the app’s windows.

struct WindowListOptions

This constant indicates a window ordering.

