

- AppKit
- NSView
-  addTrackingRect(\_:owner:userData:assumeInside:) 

Instance Method

# addTrackingRect(\_:owner:userData:assumeInside:)

Establishes an area for tracking mouse-entered and mouse-exited events within the view and returns a tag that identifies the tracking rectangle.

macOS

``` source
@MainActor
func addTrackingRect(
    _ rect: NSRect,
    owner: Any,
    userData data: UnsafeMutableRawPointer?,
    assumeInside flag: Bool
) -> NSView.TrackingRectTag
```

## Parameters 

`rect`  

A rectangle that defines a region of the view for tracking mouse-entered and mouse-exited events.

`owner`  

The object that gets sent the event messages. It can be the view itself or some other object (such as an NSCursor or a custom drawing tool object), as long as it responds to both mouseEntered(with:) and mouseExited(with:).

`data`  

Data stored in the NSEvent object for each tracking event.

`flag`  

If true, the first event will be generated when the cursor leaves `aRect`, regardless if the cursor is inside `aRect` when the tracking rectangle is added. If false the first event will be generated when the cursor leaves `aRect` if the cursor is initially inside `aRect`, or when the cursor enters `aRect` if the cursor is initially outside `aRect`. You usually want to set this flag to false.

## Return Value

A tag that identifies the tracking rectangle. It is stored in the associated NSEvent objects and can be used to remove the tracking rectangle.

## Discussion

Tracking rectangles provide a general mechanism that can be used to trigger actions based on the cursor location (for example, a status bar or hint field that provides information on the item the cursor lies over). To simply change the cursor over a particular area, use addCursorRect(_:cursor:). If you must use tracking rectangles to change the cursor, the NSCursor class specification describes the additional methods that must be invoked to change cursors by using tracking rectangles.

In macOS 10.5 and later, tracking areas provide a greater range of functionality (see addTrackingArea(_:)).

## See Also

### Related Documentation

func addTrackingArea(NSTrackingArea)

Adds a given tracking area to the view.

var userData: UnsafeMutableRawPointer?

The data associated with a mouse-tracking event.

### Managing Tracking Rectangles

func removeTrackingRect(NSView.TrackingRectTag)

Removes the tracking rectangle identified by a tag.

typealias TrackingRectTag

This type describes the rectangle used to track the mouse.

