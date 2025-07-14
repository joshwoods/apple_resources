

- AppKit
- NSWindow
-  deminiaturize(\_:) 

Instance Method

# deminiaturize(\_:)

De-minimizes the window.

macOS

``` source
@MainActor
func deminiaturize(_ sender: Any?)
```

## Parameters 

`sender`  

The message’s sender.

## Discussion

Invoke this method to programmatically deminimize a minimized window in the Dock.

## See Also

### Related Documentation

var styleMask: NSWindow.StyleMask

Flags that describe the window’s current style, such as if it’s resizable or in full-screen mode.

### Minimizing Windows

var isMiniaturized: Bool

A Boolean value that indicates whether the window is minimized.

func performMiniaturize(Any?)

Simulates the user clicking the minimize button by momentarily highlighting the button, then minimizing the window.

func miniaturize(Any?)

Removes the window from the screen list and displays the minimized window in the Dock.

var miniwindowImage: NSImage?

The custom miniaturized window image of the window.

var miniwindowTitle: String!

The title displayed in the window’s minimized window.

