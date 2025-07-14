

- AppKit
- NSWindow
-  performMiniaturize(\_:) 

Instance Method

# performMiniaturize(\_:)

Simulates the user clicking the minimize button by momentarily highlighting the button, then minimizing the window.

macOS

``` source
@MainActor
func performMiniaturize(_ sender: Any?)
```

## Parameters 

`sender`  

The message’s sender.

## Discussion

If the window doesn’t have a minimize button or can’t be minimized for some reason, the system emits the alert sound.

## See Also

### Related Documentation

var styleMask: NSWindow.StyleMask

Flags that describe the window’s current style, such as if it’s resizable or in full-screen mode.

func close()

Removes the window from the screen.

func performClose(Any?)

Simulates the user clicking the close button by momentarily highlighting the button and then closing the window.

### Minimizing Windows

var isMiniaturized: Bool

A Boolean value that indicates whether the window is minimized.

func miniaturize(Any?)

Removes the window from the screen list and displays the minimized window in the Dock.

func deminiaturize(Any?)

De-minimizes the window.

var miniwindowImage: NSImage?

The custom miniaturized window image of the window.

var miniwindowTitle: String!

The title displayed in the window’s minimized window.

