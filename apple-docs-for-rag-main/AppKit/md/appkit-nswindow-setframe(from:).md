

- AppKit
- NSWindow
-  setFrame(from:) 

Instance Method

# setFrame(from:)

Sets the window’s frame rectangle from a given string representation.

macOS

``` source
@MainActor
func setFrame(from string: NSWindow.PersistableFrameDescriptor)
```

## Parameters 

`string`  

A string representation of a frame rectangle, previously accessed using frameDescriptor.

## Discussion

If the window is not resizable, this method will not resize the window. The frame is constrained according to the window’s minimum and maximum size settings. This method causes a windowWillResize(_:to:) message to be sent to the delegate.

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

typealias FrameAutosaveName

The type of a window’s frame autosave name.

var frameDescriptor: NSWindow.PersistableFrameDescriptor

A string representation of the window’s frame rectangle.

typealias PersistableFrameDescriptor

The type of a window’s frame descriptor.

