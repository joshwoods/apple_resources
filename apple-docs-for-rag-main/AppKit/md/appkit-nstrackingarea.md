

- AppKit
-  NSTrackingArea 

Class

# NSTrackingArea

A region of a view that generates mouse-tracking and cursor-update events when the pointer is over that region.

macOS 10.5+

``` source
class NSTrackingArea
```

## Overview

When creating a tracking-area object, you specify a rectangle (in the view’s coordinate system), an owning object, and one or more options, along with (optionally) a dictionary of data. After it’s created, you add the tracking-area object to a view using the addTrackingArea(_:) method. Depending on the options specified, the owner of the tracking area receives mouseEntered(with:), mouseExited(with:), mouseMoved(with:), and cursorUpdate(with:) messages when the mouse cursor enters, moves within, and leaves the tracking area. Currently the tracking area is restricted to rectangles.

An NSTrackingArea object belongs to its view rather than to its window. Consequently, you can add and remove tracking rectangles without needing to worry if the view has been added to a window. In addition, this design makes it possible for the AppKit to compute the geometry of tracking areas automatically when a view moves and, in some cases, when a view changes size.

Using NSTrackingArea, you can configure the scope of activity for mouse tracking. There are four options:

- The tracking area is active only when the view is first responder.

- The tracking area is active when the view is in the key window.

- The tracking area is active when the application is active.

- The tracking area is active always (even when the application is inactive).

Other options for NSTrackingArea objects include specifying that the tracking area should be synchronized with the visible rectangle of the view (visibleRect) and for generating `mouseEntered:` and `mouseExited`: events when the mouse is dragged.

Other NSView methods related to NSTrackingArea objects (in addition to addTrackingArea(_:)) include removeTrackingArea(_:) and updateTrackingAreas(). Views can override the latter method to recompute and replace their NSTrackingArea objects in certain situations, such as a change in the size of the `visibleRect`.

## Topics

### Initializing the Tracking-Area Object

init(rect: NSRect, options: NSTrackingArea.Options, owner: Any?, userInfo: [AnyHashable : Any]?)

Initializes and returns an object defining a region of a view to receive mouse-tracking events, mouse-moved events, cursor-update events, or possibly all these events.

### Getting Object Attributes

var options: NSTrackingArea.Options

The options specified for the receiver.

var owner: AnyObject?

The object owning the receiver, which is the recipient of mouse-tracking, mouse-movement, and cursor-update messages.

var rect: NSRect

The rectangle defining the area encompassed by the receiver.

var userInfo: [AnyHashable : Any]?

The dictionary containing the data associated with the receiver when it was created.

### Constants

struct Options

The data type defined for the constants specified in the `options` parameter of init(rect:options:owner:userInfo:). These constants are described below; you can specify multiple constants by performing a bitwise-OR operation with them. In particular, you must supply one or more of the tracking-type constants (that is, mouseEnteredAndExited, mouseMoved, and cursorUpdate) and one of the active constants (that is, activeWhenFirstResponder, activeInKeyWindow, activeInActiveApp, and activeAlways). In addition, you may specify any of the behavior constants (that is, assumeInside, inVisibleRect, and enabledDuringMouseDrag).

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Cursors

class NSCursor

A pointer (also called a cursor).

