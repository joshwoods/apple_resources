

- AppKit
- NSWindow
-  miniaturize(\_:) 

Instance Method

# miniaturize(\_:)

Removes the window from the screen list and displays the minimized window in the Dock.

macOS

``` source
@MainActor
func miniaturize(_ sender: Any?)
```

## Parameters 

`sender`  

The message’s sender.

## See Also

### Minimizing Windows

var isMiniaturized: Bool

A Boolean value that indicates whether the window is minimized.

func performMiniaturize(Any?)

Simulates the user clicking the minimize button by momentarily highlighting the button, then minimizing the window.

func deminiaturize(Any?)

De-minimizes the window.

var miniwindowImage: NSImage?

The custom miniaturized window image of the window.

var miniwindowTitle: String!

The title displayed in the window’s minimized window.

