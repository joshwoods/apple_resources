

- AppKit
- NSApplication
-  mainWindow 

Instance Property

# mainWindow

The app’s main window.

macOS

``` source
@MainActor
weak var mainWindow: NSWindow? { get }
```

## Discussion

The value in this property is `nil` when the app’s storyboard or nib file has not yet finished loading. It might also be `nil` when the app is inactive or hidden.

## See Also

### Related Documentation

var isMainWindow: Bool

A Boolean value that indicates whether the window is the application’s main window.

### Managing App Windows

var keyWindow: NSWindow?

The window that currently receives keyboard events.

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

