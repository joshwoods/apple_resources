

- AppKit
- NSApplication
-  NSApplication.WindowListOptions 

Structure

# NSApplication.WindowListOptions

This constant indicates a window ordering.

macOS 10.12+

``` source
struct WindowListOptions
```

## Topics

### Options

static var orderedFrontToBack: NSApplication.WindowListOptions

The app’s onscreen windows in front-to-back order. By default, windows is used.

### Initializers

init(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

func enumerateWindows(options: NSApplication.WindowListOptions, using: (NSWindow, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a block for each of the app’s windows.

