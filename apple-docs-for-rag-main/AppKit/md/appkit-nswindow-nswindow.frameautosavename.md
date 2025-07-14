

- AppKit
- NSWindow
-  NSWindow.FrameAutosaveName 

Type Alias

# NSWindow.FrameAutosaveName

The type of a window’s frame autosave name.

macOS

``` source
typealias FrameAutosaveName = String
```

## See Also

### Managing Window Frames in User Defaults

class func removeFrame(usingName: NSWindow.FrameAutosaveName)

Removes the frame data stored under a given name from the application’s user defaults.

func setFrameUsingName(NSWindow.FrameAutosaveName) -> Bool

Sets the window’s frame rectangle by reading the rectangle data stored under a given name from the defaults system.

func setFrameUsingName(NSWindow.FrameAutosaveName, force: Bool) -> Bool

Sets the window’s frame rectangle by reading the rectangle data stored under a given name from the defaults system. Can operate on non-resizable windows.

func saveFrame(usingName: NSWindow.FrameAutosaveName)

Saves the window’s frame rectangle in the user defaults system under a given name.

func setFrameAutosaveName(NSWindow.FrameAutosaveName) -> Bool

Sets the name AppKit uses to automatically save the window’s frame rectangle data in the defaults system.

var frameAutosaveName: NSWindow.FrameAutosaveName

The name used to automatically save the window’s frame rectangle data in the defaults system.

var frameDescriptor: NSWindow.PersistableFrameDescriptor

A string representation of the window’s frame rectangle.

func setFrame(from: NSWindow.PersistableFrameDescriptor)

Sets the window’s frame rectangle from a given string representation.

typealias PersistableFrameDescriptor

The type of a window’s frame descriptor.

