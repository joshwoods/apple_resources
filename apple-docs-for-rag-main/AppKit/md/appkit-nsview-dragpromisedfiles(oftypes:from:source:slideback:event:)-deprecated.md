

- AppKit
- NSView
-  dragPromisedFiles(ofTypes:from:source:slideBack:event:) Deprecated

Instance Method

# dragPromisedFiles(ofTypes:from:source:slideBack:event:)

Initiates a dragging operation from the view, allowing the user to drag one or more promised files (or directories) into any application that has window or view objects that accept promised file data.

macOS 10.0–10.13Deprecated

``` source
@MainActor
func dragPromisedFiles(
    ofTypes typeArray: [String],
    from rect: NSRect,
    source sourceObject: Any,
    slideBack flag: Bool,
    event: NSEvent
) -> Bool
```

Deprecated

Use beginDraggingSession(with:event:source:) instead.

## Parameters 

`typeArray`  

An array of file types being promised. The array elements can consist of file extensions and HFS types encoded with the NSFileTypeForHFSTypeCode(_:) function. If promising a directory of files, only include the top directory in the array.

`rect`  

A rectangle that describes the position of the icon in the view’s coordinate system.

`sourceObject`  

An object that serves as the controller of the dragging operation. It must conform to the NSDraggingSource protocol, and is typically the view itself or its NSWindow object.

`flag`  

A Boolean that indicates whether the icon being dragged should slide back to its position in the view if the file isn’t accepted. The icon slides back to `aRect` if `slideBack` is true, the promised files are not accepted by the dragging destination, and the user has not disabled icon animation; otherwise it simply disappears.

`event`  

The mouse-down event object from which to initiate the drag operation. In particular, its mouse location is used for the offset of the icon being dragged.

## Return Value

true if the drag operation is initiated successfully, false otherwise.

## Discussion

This method must be invoked only within an implementation of the mouseDown(with:) method. As part of its implementation, this method invokes dragImage:at:offset:event:pasteboard:source:slideBack:.

Promised files are files that do not exist, yet, but that the drag source, `sourceObject`, promises to create at a file system location specified by the drag destination when the drag is successfully dropped.

See Drag and Drop Programming Topics for more information on dragging operations.

## See Also

### Related Documentation

func unregisterDraggedTypes()

Unregisters the view as a possible destination in a dragging session.

func registerForDraggedTypes([NSPasteboard.PasteboardType])

Registers the pasteboard types that the view will accept as the destination of an image-dragging session.

func shouldDelayWindowOrdering(for: NSEvent) -> Bool

Allows the user to drag objects from the view without activating the app or moving the window of the view forward, possibly obscuring the destination.

func beginDraggingSession(with: [NSDraggingItem], event: NSEvent, source: any NSDraggingSource) -> NSDraggingSession

Initiates a dragging session with a group of dragging items.

### Methods

func lockFocus()

Locks the focus on the view, so subsequent commands take effect in the view’s window and coordinate system.

Deprecated

func lockFocusIfCanDraw() -> Bool

Locks the focus to the view atomically if the `canDraw` method returns true and returns the value of `canDraw`.

Deprecated

func lockFocusIfCanDraw(in: NSGraphicsContext) -> Bool

Locks the focus to the view atomically if drawing can occur in the specified graphics context.

Deprecated

func unlockFocus()

Unlocks focus from the current view.

Deprecated

func scroll(NSRect, by: NSSize)

Copies the visible portion of the view’s rendered image within a region and lays that portion down again at a specified offset .

Deprecated

func shouldDrawColor() -> Bool

Returns a Boolean value indicating whether the view is being drawn to an environment that supports color.

Deprecated

func allocateGState()

Causes the view to maintain a private graphics state object, which encapsulates all parameters of the graphics environment.

Deprecated

func gState() -> Int

Returns the identifier for the view’s graphics state object, or 0 if the view doesn’t have a graphics state object.

Deprecated

func setUpGState()

Overridden by subclasses to (re)initialize the view’s graphics state object.

Deprecated

func renewGState()

Invalidates the view’s graphics state object, if it has one.

Deprecated

func releaseGState()

Frees the view’s graphics state object, if it has one.

Deprecated

func dragFile(String, from: NSRect, slideBack: Bool, event: NSEvent) -> Bool

Initiates a dragging operation from the view, allowing the user to drag a file icon to any application that has window or view objects that accept files.

Deprecated

