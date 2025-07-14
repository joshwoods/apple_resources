

- AppKit
- NSApplication
-  enumerateWindows(options:using:) 

Instance Method

# enumerateWindows(options:using:)

Executes a block for each of the app’s windows.

macOS 10.12+

``` source
@MainActor
func enumerateWindows(
    options: NSApplication.WindowListOptions = [],
    using block: (NSWindow, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`options`  

A constant that indicates window ordering. See NSApplication.WindowListOptions for possible values.

`block`  

The block to execute for each window. The block takes the following parameters:

window  
The window for which to execute the block.

stop  
A Boolean value that stops the enumeration early when set to true (the default value is false).

## See Also

### Managing App Windows

var keyWindow: NSWindow?

The window that currently receives keyboard events.

var mainWindow: NSWindow?

The app’s main window.

func window(withWindowNumber: Int) -> NSWindow?

Returns the window corresponding to the specified window number.

var windows: [NSWindow]

An array of the app’s window objects.

func makeWindowsPerform(Selector, inOrder: Bool) -> NSWindow?

Sends the specified message to each of the app’s window objects until one returns a non-`nil` value.

Deprecated

struct WindowListOptions

This constant indicates a window ordering.

