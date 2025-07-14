

- AppKit
- NSApplication
-  window(withWindowNumber:) 

Instance Method

# window(withWindowNumber:)

Returns the window corresponding to the specified window number.

macOS

``` source
@MainActor
func window(withWindowNumber windowNum: Int) -> NSWindow?
```

## Parameters 

`windowNum`  

The unique window number associated with the desired NSWindow object.

## Return Value

The desired window object or `nil` if the window could not be found.

## Discussion

window(withWindowNumber:) may return `nil` for window numbers found using windowNumbers(options:) if there is no corresponding window object owned by your app—for example, the menu bar.

## See Also

### Managing App Windows

var keyWindow: NSWindow?

The window that currently receives keyboard events.

var mainWindow: NSWindow?

The app’s main window.

var windows: [NSWindow]

An array of the app’s window objects.

func makeWindowsPerform(Selector, inOrder: Bool) -> NSWindow?

Sends the specified message to each of the app’s window objects until one returns a non-`nil` value.

Deprecated

func enumerateWindows(options: NSApplication.WindowListOptions, using: (NSWindow, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a block for each of the app’s windows.

struct WindowListOptions

This constant indicates a window ordering.

