

- AppKit
- NSTrackingArea
- NSTrackingArea.Options
-  activeAlways 

Type Property

# activeAlways

The owner receives messages regardless of first-responder status, window status, or application status. The cursorUpdate(with:) message is *not* sent when the cursorUpdate option is specified along with this constant. This value specifies when the tracking area defined by an NSTrackingArea object is active.

macOS

``` source
static var activeAlways: NSTrackingArea.Options { get }
```

## See Also

### Constants

static var mouseEnteredAndExited: NSTrackingArea.Options

The owner of the tracking area receives mouseEntered(with:) when the mouse cursor enters the area and mouseExited(with:) events when the mouse leaves the area. This value specifies a type of tracking area.

static var mouseMoved: NSTrackingArea.Options

The owner of the tracking area receives mouseMoved(with:) messages while the mouse cursor is within the area. This value specifies a type of tracking area.

static var cursorUpdate: NSTrackingArea.Options

A tracking option that receives events when the mouse cursor enters and exits the tracking area.

static var activeWhenFirstResponder: NSTrackingArea.Options

The owner receives messages when the view is the first responder. This value specifies when the tracking area defined by an NSTrackingArea object is active.

static var activeInKeyWindow: NSTrackingArea.Options

The owner receives messages when the view is in the key window. This value specifies when the tracking area defined by an NSTrackingArea object is active.

static var activeInActiveApp: NSTrackingArea.Options

The owner receives messages when the application is active. This value specifies when the tracking area defined by an NSTrackingArea object is active.

static var assumeInside: NSTrackingArea.Options

The first event is generated when the cursor leaves the tracking area, regardless if the cursor is inside the area when the `NSTrackingArea` is added to a view. If this option is not specified, the first event is generated when the cursor leaves the tracking area if the cursor is initially inside the area, or when the cursor enters the area if the cursor is initially outside it. Generally, you do not want to request this behavior. This value specifies a behavior of the tracking area defined by the NSTrackingArea.

static var inVisibleRect: NSTrackingArea.Options

Mouse tracking occurs only in the visible rectangle of the view—in other words, that region of the tracking rectangle that is unobscured. Otherwise, the entire tracking area is active regardless of overlapping views. The `NSTrackingArea` object is automatically synchronized with changes in the view’s visible area (visibleRect) and the value returned from rect is ignored. This value specifies a behavior of the tracking area defined by the NSTrackingArea.

static var enabledDuringMouseDrag: NSTrackingArea.Options

The owner receives NSMouseEntered events when the mouse cursor is dragged into the tracking area. If this option is not specified, the owner receives mouse-entered events when the mouse is moved (no buttons pressed) into the tracking area and on NSLeftMouseUp events after a mouse drag.

