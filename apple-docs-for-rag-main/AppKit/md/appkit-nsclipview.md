

- AppKit
-  NSClipView 

Class

# NSClipView

An object that clips a document view to a scroll view’s frame.

macOS

``` source
@MainActor
class NSClipView
```

## Overview

An NSClipView holds the document view of an NSScrollView, clipping the document view to its frame, handling the details of scrolling in an efficient manner, and updating the NSScrollView when the document view’s size or position changes.

You don’t typically use the NSClipView class directly; it’s provided primarily as the scrolling machinery for the NSScrollView class. However, you might use the NSClipView class to implement a class similar to NSScrollView.

### Interaction with NSScrollView

When using an NSClipView within an NSScrollView (the usual configuration), you should access the NSScrollView properties that control background drawing state, rather than accessing these properties of the NSClipView. This recommendation applies to the following properties:

- backgroundColor

- drawsBackground

The NSClipView methods are intended for when the NSClipView is used independently of a containing NSScrollView. In the usual case, NSScrollView should be allowed to manage the background-drawing properties of its associated NSClipView.

There is only one background-drawing state per NSScrollView/NSClipView pair. The two objects do not maintain independent and distinct drawsBackground and backgroundColor properties; rather, the accessors for these properties on NSScrollView largely defer to the associated NSClipView and allow the NSClipView to maintain the state. Note that this state is not cached by the NSScrollView object.

It is also important to note that setting drawsBackground to false in an NSScrollView has the added effect of setting the NSClipView property copiesOnScroll to false. The side effect of setting the drawsBackground property directly to the NSClipView is the appearance of “trails” (vestiges of previous drawing) in the document view as it is scrolled.

## Topics

### Setting the Document View

var documentView: NSView?

The clip view’s document view.

### Scrolling

func scroll(to: NSPoint)

Changes the origin of the clip view’s bounds rectangle to `newOrigin`.

func autoscroll(with: NSEvent) -> Bool

Scrolls the clip view proportionally to `theEvent`’s distance outside of it.

func constrainScroll(NSPoint) -> NSPoint

Returns a scroll point adjusted from the proposed new origin, if necessary, to guarantee the view will lie within its document view.

Deprecated

func constrainBoundsRect(NSRect) -> NSRect

Constrains the bounds of the clip view while the user is magnifying and scrolling.

### Determining Scrolling Efficiency

var copiesOnScroll: Bool

A Boolean value that indicates if the clip view copies rendered images while scrolling.

Deprecated

### Accessing the Content Insets

var contentInsets: NSEdgeInsets

The distance that the content view is inset from the enclosing scroll view.

var automaticallyAdjustsContentInsets: Bool

A Boolean value that indicates if the clip view automatically accounts for other scroll view subviews.

### Accessing the Visible Portion

var documentRect: NSRect

The rectangle defining the document view’s frame, adjusted to the size of the clip view if the document view is smaller.

var documentVisibleRect: NSRect

The exposed rectangle of the clip view’s document view, in the document view’s own coordinate system.

### Setting the Document Cursor

var documentCursor: NSCursor?

The cursor object used when the pointer lies over the view.

### Working with Background Color

var drawsBackground: Bool

A Boolean value that indicates if the clip view draws its background color.

var backgroundColor: NSColor

The color of the clip view’s background.

### Overriding NSView Methods

func viewBoundsChanged(Notification)

Handles an boundsDidChangeNotification, passed in the `aNotification` argument, by updating a containing NSScrollView based on the new bounds.

func viewFrameChanged(Notification)

Handles an frameDidChangeNotification, passed in the `aNotification` argument, by updating a containing NSScrollView based on the new frame.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Views

class NSScrollView

A view that displays a portion of a document view and provides scroll bars that allow the user to move the document view within the scroll view.

class NSScroller

An object that controls scrolling of a document view within a scroll view or other type of container view.

