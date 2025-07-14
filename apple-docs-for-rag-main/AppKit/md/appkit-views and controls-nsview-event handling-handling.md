

- AppKit
- Views and Controls
- NSView
-  Event Handling 

API Collection

# Event Handling

Respond to mouse, keyboard, touch, and tablet events and gestures that originate inside your view.

## Topics

### Handling Events in the View

func acceptsFirstMouse(for: NSEvent?) -> Bool

Overridden by subclasses to return true if the view should be sent a mouseDown(with:) message for an initial mouse-down event, false if not.

func hitTest(NSPoint) -> NSView?

Returns the farthest descendant of the view in the view hierarchy (including itself) that contains a specified point, or `nil` if that point lies completely outside the view.

func isMousePoint(NSPoint, in: NSRect) -> Bool

Returns whether a region of the view contains a specified point, accounting for whether the view is flipped or not.

func performKeyEquivalent(with: NSEvent) -> Bool

Implemented by subclasses to respond to key equivalents (also known as keyboard shortcuts).

func rightMouseDown(with: NSEvent)

Informs the receiver that the user has pressed the right mouse button.

var mouseDownCanMoveWindow: Bool

A Boolean value indicating whether the view can pass mouse down events through to its superviews.

var inputContext: NSTextInputContext?

The text input context object for the view.

### Handling Touch Events

var allowedTouchTypes: NSTouch.TouchTypeMask

The types of touch interactions the view allows.

var wantsRestingTouches: Bool

A Boolean value indicating whether the view wants resting touches.

var candidateListTouchBarItem: NSCandidateListTouchBarItem&lt;AnyObject>?

### Managing Gesture Recognizers

var gestureRecognizers: [NSGestureRecognizer]

The gesture recognize objects currently attached to the view.

func addGestureRecognizer(NSGestureRecognizer)

Attaches a gesture recognizer to the view.

func removeGestureRecognizer(NSGestureRecognizer)

Detaches a gesture recognizer from the view.

### Managing the Key-View Loop

var canBecomeKeyView: Bool

A Boolean value indicating whether the view can become key view.

var needsPanelToBecomeKey: Bool

A Boolean value indicating whether the view needs its panel to become the key window before it can handle keyboard input and navigation.

var nextKeyView: NSView?

The view object that follows the current view in the key view loop.

var nextValidKeyView: NSView?

The closest view object in the key view loop that follows the current view in the key view loop and accepts first responder status.

var previousKeyView: NSView?

The view object preceding the current view in the key view loop.

var previousValidKeyView: NSView?

The closest view object in the key view loop that precedes the current view and accepts first responder status.

### Handling Smart Magnification

func rectForSmartMagnification(at: NSPoint, in: NSRect) -> NSRect

Returns the appropriate rectangle to use when magnifying around the specified point.

### Managing Tracking Areas

func addTrackingArea(NSTrackingArea)

Adds a given tracking area to the view.

func removeTrackingArea(NSTrackingArea)

Removes a given tracking area from the view.

var trackingAreas: [NSTrackingArea]

An array of the view’s tracking areas.

func updateTrackingAreas()

Invoked automatically when the view’s geometry changes such that its tracking areas need to be recalculated.

class let didUpdateTrackingAreasNotification: NSNotification.Name

Posted whenever a view recalculates its tracking areas.

### Managing Tracking Rectangles

func addTrackingRect(NSRect, owner: Any, userData: UnsafeMutableRawPointer?, assumeInside: Bool) -> NSView.TrackingRectTag

Establishes an area for tracking mouse-entered and mouse-exited events within the view and returns a tag that identifies the tracking rectangle.

func removeTrackingRect(NSView.TrackingRectTag)

Removes the tracking rectangle identified by a tag.

typealias TrackingRectTag

This type describes the rectangle used to track the mouse.

### Scrolling the View

func prepareContent(in: NSRect)

Prepares the overdraw region for drawing.

var preparedContentRect: NSRect

The portion of the view that has been rendered and is available for responsive scrolling.

func scroll(NSPoint)

Scrolls the view’s closest ancestor NSClipView object so a point in the view lies at the origin of the clip view’s bounds rectangle.

func scrollToVisible(NSRect) -> Bool

Scrolls the view’s closest ancestor NSClipView object the minimum distance needed so a specified region of the view becomes visible in the clip view.

func autoscroll(with: NSEvent) -> Bool

Scrolls the view’s closest ancestor NSClipView object proportionally to the distance of an event that occurs outside of it.

func adjustScroll(NSRect) -> NSRect

Overridden by subclasses to modify a given rectangle, returning the altered rectangle.

var enclosingScrollView: NSScrollView?

The nearest ancestor scroll view that contains the current view.

func scroll(NSClipView, to: NSPoint)

Notifies the superview of a clip view that the clip view needs to reset the origin of its bounds rectangle.

func reflectScrolledClipView(NSClipView)

Notifies a clip view’s superview that either the clip view’s bounds rectangle or the document view’s frame rectangle has changed, and that any indicators of the scroll position need to be adjusted.

class var isCompatibleWithResponsiveScrolling: Bool

A Boolean value that indicates whether views support responsive scrolling.

### Configuring Pressure

var pressureConfiguration: NSPressureConfiguration?

Configures the behavior and progression of the Force Touch trackpad when responding to touch input produced by the user when the cursor is over the view.

### Dragging Operations

func registerForDraggedTypes([NSPasteboard.PasteboardType])

Registers the pasteboard types that the view will accept as the destination of an image-dragging session.

func unregisterDraggedTypes()

Unregisters the view as a possible destination in a dragging session.

var registeredDraggedTypes: [NSPasteboard.PasteboardType]

The array of pasteboard drag types that the view can accept.

func beginDraggingSession(with: [NSDraggingItem], event: NSEvent, source: any NSDraggingSource) -> NSDraggingSession

Initiates a dragging session with a group of dragging items.

func shouldDelayWindowOrdering(for: NSEvent) -> Bool

Allows the user to drag objects from the view without activating the app or moving the window of the view forward, possibly obscuring the destination.

