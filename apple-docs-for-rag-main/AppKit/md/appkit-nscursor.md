

- AppKit
-  NSCursor 

Class

# NSCursor

A pointer (also called a cursor).

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.0+

``` source
class NSCursor
```

## Overview

The following table shows and describes the system cursors, and indicates the class method for obtaining them:

| Cursor | Description |
|----|----|
|  | The arrow cursor (arrow) |
|  | The I-beam cursor for indicating insertion points (iBeam) |
|  | The cross-hair cursor (crosshair) |
|  | The closed-hand cursor (closedHand) |
|  | The open-hand cursor (openHand) |
|  | The pointing-hand cursor (pointingHand) |
|  | The resize-left cursor (resizeLeft) |
|  | The resize-right cursor (resizeRight) |
|  | The resize-left-and-right cursor (resizeLeftRight) |
|  | The resize-up cursor (resizeUp) |
|  | The resize-down cursor (resizeDown) |
|  | The resize-up-and-down cursor (resizeUpDown) |
|  | The disappearing item cursor (disappearingItem) |
|  | The I-Beam text cursor for vertical layout (iBeamCursorForVerticalLayout). |
|  | The not allowed cursor (operationNotAllowed). |
|  | The drag link cursor (dragLink). |
|  | The drag copy cursor (dragCopy). |
|  | The contextual menu cursor (contextualMenu). |

In macOS 10.3 and later, cursor size is no longer limited to 16 by 16 pixels.

### Cursor Rectangles

In Cocoa, you can change the currently displayed cursor based on the position of the mouse over one of your views. You might use this technique to provide visual feedback about what actions the user can take with the mouse. For example, you might display one of the resize cursors whenever the mouse moves over a portion of your view that acts as a custom resizing handle. To set this up, you associate a cursor object with one or more cursor rectangles in the view.

Cursor rectangles are a specialized type of tracking rectangles, which are used to monitor the mouse location in a view. Views implement cursor rectangles using tracking rectangles but provide methods for setting and refreshing cursor rectangles that are distinct from the generic tracking rectangle interface. For information on how to set up cursor rectangles, see Mouse-Tracking and Cursor-Update Events.

### Balancing Cursor Hiding and Unhiding

Each call to hide() cursor must have a corresponding unhide() call. For example,

```
[NSCursor hide];
[NSCursor hide];
// ...
[NSCursor unhide];
```

Will result in the cursor still being hidden because the `hide` and `unhide` method invocations are not balanced. Instead you must balance the method calls, such as in the following example:

```
[NSCursor hide];
[NSCursor hide];
// ...
[NSCursor unhide];
[NSCursor unhide];
```

There are corresponding cursor `hide` and `unhide` calls, thus the cursor will become visible.

## Topics

### Initializing a New Cursor

init(image: UIImage, hotSpot: NSPoint)

Initializes a cursor with the given image and hot spot.

convenience init(image: NSImage, foregroundColorHint: NSColor?, backgroundColorHint: NSColor?, hotSpot: NSPoint)

Initializes the cursor with the specified image and hot spot.

Deprecated

### Setting Cursor Attributes

var image: UIImage

The cursor’s image.

var hotSpot: NSPoint

The position of the click location within the cursor.

class func hide()

Makes the current cursor invisible.

class func unhide()

Negates an earlier call to hide() by showing the current cursor.

class func setHiddenUntilMouseMoves(Bool)

Sets whether the cursor is hidden until the mouse moves.

### Controlling Which Cursor Is Current

class func pop()

Pops the current cursor off the top of the stack.

func pop()

Sends a pop() message to the receiver’s class.

func push()

Puts the receiver on top of the cursor stack and makes it the current cursor.

func set()

Makes the receiver the current cursor.

func mouseEntered(with: NSEvent)

Automatically sent to the receiver when the cursor enters a cursor rectangle owned by the receiver.

Deprecated

func setOnMouseEntered(Bool)

Specifies whether the receiver accepts mouseEntered(with:) events.

Deprecated

var isSetOnMouseEntered: Bool

A Boolean value indicating whether the receiver becomes current on receiving a mouseEntered(with:) message.

Deprecated

func mouseExited(with: NSEvent)

Automatically sent to the receiver when the cursor exits a cursor rectangle owned by the receiver.

Deprecated

func setOnMouseExited(Bool)

Sets whether the receiver accepts mouseExited(with:) events.

Deprecated

var isSetOnMouseExited: Bool

A Boolean value indicating whether the receiver becomes current when it receives a mouseExited(with:) message.

Deprecated

### Retrieving Cursor Instances

class var current: NSCursor

Returns the application’s current cursor.

class var currentSystem: NSCursor?

Returns the current system cursor.

class var arrow: NSCursor

Returns the default cursor, the arrow cursor.

class var contextualMenu: NSCursor

Returns the contextual menu system cursor.

class var closedHand: NSCursor

Returns the closed-hand system cursor.

class var crosshair: NSCursor

Returns the cross-hair system cursor.

class var disappearingItem: NSCursor

Returns a cursor indicating that the current operation will result in a disappearing item.

class var dragCopy: NSCursor

Returns a cursor indicating that the current operation will result in a copy action.

class var dragLink: NSCursor

Returns a cursor indicating that the current operation will result in a link action.

class var iBeam: NSCursor

Returns a cursor that looks like a capital I with a tiny crossbeam at its middle.

class var openHand: NSCursor

Returns the open-hand system cursor.

class var operationNotAllowed: NSCursor

Returns the operation not allowed cursor.

class var pointingHand: NSCursor

Returns the pointing-hand system cursor.

class var resizeDown: NSCursor

Returns the resize-down system cursor.

class var resizeLeft: NSCursor

Returns the resize-left system cursor.

class var resizeLeftRight: NSCursor

Returns the resize-left-and-right system cursor.

class var resizeRight: NSCursor

Returns the resize-right system cursor.

class var resizeUp: NSCursor

Returns the resize-up system cursor.

class var resizeUpDown: NSCursor

Returns the resize-up-and-down system cursor.

class var iBeamCursorForVerticalLayout: NSCursor

Returns the cursor for editing vertical layout text.

### Constants

AppKit Versions for NSCursor Bug Fixes

The version of the AppKit framework containing a specific bug fix.

### Initializers

init(coder: NSCoder)

### Type Properties

class var columnResize: NSCursor

Returns the cursor for resizing a column (vertical divider) in either direction.

class var rowResize: NSCursor

Returns the cursor for resizing a row (horizontal divider) in either direction.

class var zoomIn: NSCursor

Returns the zoom-in cursor.

class var zoomOut: NSCursor

Returns the zoom-out cursor.

### Type Methods

class func columnResize(directions: NSHorizontalDirection.Set) -> NSCursor

Returns the cursor for resizing a column (vertical divider) in the specified direction.

class func frameResize(position: NSCursor.FrameResizePosition, directions: NSCursor.FrameResizeDirection.Set) -> NSCursor

Returns the cursor for resizing a rectangular frame from the specified edge or corner.

class func javaBusyButClickable() -> NSCursor!

class func javaMove() -> NSCursor!

class func javaResizeNE() -> NSCursor!

class func javaResizeNW() -> NSCursor!

class func javaResizeSE() -> NSCursor!

class func javaResizeSW() -> NSCursor!

class func javaSetAllowsCursorSet(inBackground: Bool)

class func rowResize(directions: NSVerticalDirection.Set) -> NSCursor

Returns the cursor for resizing a row (horizontal divider) in the specified direction.

### Enumerations

enum FrameResizeDirection

The direction in which a rectangular frame can be resized.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Cursors

class NSTrackingArea

A region of a view that generates mouse-tracking and cursor-update events when the pointer is over that region.

