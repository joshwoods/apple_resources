

- AppKit
- NSWindowController
-  showWindow(\_:) 

Instance Method

# showWindow(\_:)

Displays the window associated with the receiver.

macOS

``` source
@IBAction @MainActor
func showWindow(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message; can be `nil`.

## Discussion

If the window is an NSPanel object and has its becomesKeyOnlyIfNeeded flag set to true, the window is displayed in front of all other windows but is not made key; otherwise it is displayed in front and is made key. This method is useful for menu actions.

## See Also

### Related Documentation

func orderFront(Any?)

Moves the window to the front of its level in the screen list, without changing either the key window or the main window.

func makeKeyAndOrderFront(Any?)

Moves the window to the front of the screen list, within its level, and makes it the key window; that is, it shows the window.

### Loading and Displaying the Window

func loadWindow()

Loads the receiver’s window from the nib file.

var isWindowLoaded: Bool

A Boolean value that indicates whether the nib file containing the receiver’s window has been loaded.

var window: NSWindow?

The window owned by the receiver.

func windowDidLoad()

Sent after the window owned by the receiver has been loaded.

func windowWillLoad()

Sent before the window owned by the receiver is loaded.

