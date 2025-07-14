

- AppKit
- NSApplication
-  arrangeInFront(\_:) 

Instance Method

# arrangeInFront(\_:)

Arranges windows listed in the Window menu in front of all other windows.

macOS

``` source
@MainActor
func arrangeInFront(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent the command.

## Discussion

Windows associated with the app but not listed in the Window menu are not ordered to the front.

## See Also

### Related Documentation

func addWindowsItem(NSWindow, title: String, filename: Bool)

Adds an item to the Window menu for a given window.

func removeWindowsItem(NSWindow)

Removes the Window menu item for a given window.

func makeKeyAndOrderFront(Any?)

Moves the window to the front of the screen list, within its level, and makes it the key window; that is, it shows the window.

### Managing Window Layers

func preventWindowOrdering()

Suppresses the usual window ordering in handling the most recent mouse-down event.

