

- AppKit
- NSWindow
-  setFrameUsingName(\_:force:) 

Instance Method

# setFrameUsingName(\_:force:)

Sets the window’s frame rectangle by reading the rectangle data stored under a given name from the defaults system. Can operate on non-resizable windows.

macOS

``` source
@MainActor
func setFrameUsingName(
    _ name: NSWindow.FrameAutosaveName,
    force: Bool
) -> Bool
```

## Parameters 

`name`  

The name of the frame to read.

`force`  

true to use setFrameUsingName(_:) on a non-resizable window; false to fail on a non-resizable window.

## Return Value

true when `name` is read and the frame is set successfully; otherwise, false.

## See Also

### Managing Window Frames in User Defaults

class func removeFrame(usingName: NSWindow.FrameAutosaveName)

Removes the frame data stored under a given name from the application’s user defaults.

func setFrameUsingName(NSWindow.FrameAutosaveName) -> Bool

Sets the window’s frame rectangle by reading the rectangle data stored under a given name from the defaults system.

func saveFrame(usingName: NSWindow.FrameAutosaveName)

Saves the window’s frame rectangle in the user defaults system under a given name.

func setFrameAutosaveName(NSWindow.FrameAutosaveName) -> Bool

Sets the name AppKit uses to automatically save the window’s frame rectangle data in the defaults system.

var frameAutosaveName: NSWindow.FrameAutosaveName

The name used to automatically save the window’s frame rectangle data in the defaults system.

typealias FrameAutosaveName

The type of a window’s frame autosave name.

var frameDescriptor: NSWindow.PersistableFrameDescriptor

A string representation of the window’s frame rectangle.

func setFrame(from: NSWindow.PersistableFrameDescriptor)

Sets the window’s frame rectangle from a given string representation.

typealias PersistableFrameDescriptor

The type of a window’s frame descriptor.

