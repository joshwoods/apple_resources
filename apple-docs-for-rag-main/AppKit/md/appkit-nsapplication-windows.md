

- AppKit
- NSApplication
-  windows 

Instance Property

# windows

An array of the app’s window objects.

macOS

``` source
@MainActor
var windows: [NSWindow] { get }
```

## Discussion

This property contains an array of NSWindow objects corresponding to all currently existing windows for the app. The array includes all onscreen and offscreen windows, whether or not they are visible on any space. There is no guarantee of the order of the windows in the array.

## See Also

### Managing App Windows

var keyWindow: NSWindow?

The window that currently receives keyboard events.

var mainWindow: NSWindow?

The app’s main window.

func window(withWindowNumber: Int) -> NSWindow?

Returns the window corresponding to the specified window number.

func makeWindowsPerform(Selector, inOrder: Bool) -> NSWindow?

Sends the specified message to each of the app’s window objects until one returns a non-`nil` value.

Deprecated

func enumerateWindows(options: NSApplication.WindowListOptions, using: (NSWindow, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a block for each of the app’s windows.

struct WindowListOptions

This constant indicates a window ordering.

