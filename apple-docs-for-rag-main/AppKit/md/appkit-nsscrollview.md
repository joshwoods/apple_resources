

- AppKit
-  NSScrollView 

Class

# NSScrollView

A view that displays a portion of a document view and provides scroll bars that allow the user to move the document view within the scroll view.

macOS

``` source
@MainActor
class NSScrollView
```

## Overview

The NSScrollView class is the central coordinator for AppKit’s scrolling machinery, which is composed of this class, and the NSClipView and NSScroller classes.

When using an NSClipView object within a scroll view (the usual configuration), you should issue messages that control background drawing state to the scroll view directly, rather than messaging the clip view.

## Topics

### Calculating Layout

class func frameSize(forContentSize: NSSize, horizontalScrollerClass: AnyClass?, verticalScrollerClass: AnyClass?, borderType: NSBorderType, controlSize: NSControl.ControlSize, scrollerStyle: NSScroller.Style) -> NSSize

Returns the frame size of a scroll view that contains a content view with the specified size.

class func contentSize(forFrameSize: NSSize, horizontalScrollerClass: AnyClass?, verticalScrollerClass: AnyClass?, borderType: NSBorderType, controlSize: NSControl.ControlSize, scrollerStyle: NSScroller.Style) -> NSSize

Returns the content size calculated from the frame size and the specified specifications.

### Determining Component Sizes

var contentSize: NSSize

The size of the scroll view’s content view.

var documentVisibleRect: NSRect

The portion of the document view, in its own coordinate system, visible through the scroll view’s content view.

### Managing Graphics Attributes

var backgroundColor: NSColor

The color of the content view’s background.

var drawsBackground: Bool

A Boolean that indicates whether the scroll view draws its background.

var borderType: NSBorderType

A value that specifies the appearance of the scroll view’s border.

var documentCursor: NSCursor?

The content view’s document cursor.

### Managing the Views

var contentView: NSClipView

The scroll view’s content view, the view that clips the document view.

var documentView: NSView?

The view the scroll view scrolls within its content view.

func addFloatingSubview(NSView, for: NSEvent.GestureAxis)

Adds a floating subview to the document view.

### Managing Scrollers

var horizontalScroller: NSScroller?

The scroll view’s horizontal scroller.

var hasHorizontalScroller: Bool

A Boolean that indicates whether the scroll view has a horizontal scroller.

var verticalScroller: NSScroller?

The scroll view’s vertical scroller.

var hasVerticalScroller: Bool

A Boolean that indicates whether the scroll view has a vertical scroller.

var autohidesScrollers: Bool

A Boolean that indicates whether the scroll view automatically hides its scroll bars when they are not needed.

### Managing Rulers

class var rulerViewClass: AnyClass!

Returns the default class to be used for ruler objects in NSScrollViews.

var hasHorizontalRuler: Bool

A Boolean that indicates whether the scroll view keeps a horizontal ruler object.

var horizontalRulerView: NSRulerView?

The scroll view’s horizontal ruler view.

var hasVerticalRuler: Bool

A Boolean that indicates whether the scroll view keeps a vertical ruler object.

var verticalRulerView: NSRulerView?

The scroll view’s vertical ruler view.

var rulersVisible: Bool

A Boolean that indicates whether the scroll view displays its rulers.

### Managing Insets

var automaticallyAdjustsContentInsets: Bool

A Boolean that indicates whether the scroll view automatically adjusts its content insets.

var contentInsets: NSEdgeInsets

The distance that the scroll view’s subviews are inset from the enclosing scroll view during tiling.

var scrollerInsets: NSEdgeInsets

The distance the scrollers are inset from the edge of the scroll view.

### Scroller Style

var scrollerKnobStyle: NSScroller.KnobStyle

The knob style of scroll views that use the overlay scroller style.

var scrollerStyle: NSScroller.Style

The scroller style used by the scroll view.

### Setting Scrolling Behavior

var lineScroll: CGFloat

The scroll view’s line by line scroll amount.

var horizontalLineScroll: CGFloat

The scroll view’s horizontal line by line scroll amount.

var verticalLineScroll: CGFloat

The scroll view’s vertical line by line scroll amount.

var pageScroll: CGFloat

The amount of the document view kept visible when scrolling page by page.

var horizontalPageScroll: CGFloat

The amount of the document view kept visible when scrolling horizontally page by page.

var verticalPageScroll: CGFloat

The amount of the document view kept visible when scrolling vertically page by page.

var scrollsDynamically: Bool

A Boolean that indicates whether the scroll view redraws its document view while scrolling continuously.

func scrollWheel(with: NSEvent)

Scrolls the receiver up or down, in response to the user moving the mouse’s scroll wheel specified by `theEvent`.

### Updating Display After Scrolling

func reflectScrolledClipView(NSClipView)

Adjusts the receiver’s scrollers to reflect the size and positioning of its content view.

### Arranging Components

func tile()

Lays out the components of the receiver: the content view, the scrollers, and the ruler views.

### Find Bar Positioning

var findBarPosition: NSScrollView.FindBarPosition

The position of the find bar.

### Specifying a Document’s Predominant Scrolling Behavior

var usesPredominantAxisScrolling: Bool

A Boolean that indicates whether the scroll view uses a predominant scrolling axis for content.

### Specifying the Scroll View Elasticity

var horizontalScrollElasticity: NSScrollView.Elasticity

The scroll view’s horizontal scrolling elasticity mode.

var verticalScrollElasticity: NSScrollView.Elasticity

The scroll view’s vertical scrolling elasticity mode.

### Flashing Overlay Scroll Bars

func flashScrollers()

Flash the overlay scroll bars.

### Zooming the Scroll View

var allowsMagnification: Bool

Allows the user to magnify the scroll view.

var magnification: CGFloat

The amount by which the content is currently scaled.

func magnify(toFit: NSRect)

Magnifies the content view proportionally such that the given rectangle fits centered in the scroll view.

var maxMagnification: CGFloat

The maximum value to which the content can be magnified.

var minMagnification: CGFloat

The minimum value to which the content can be magnified.

func setMagnification(CGFloat, centeredAt: NSPoint)

Magnify the content by the given amount and center the result on the given point.

### Constants

enum Elasticity

These constants determine the elasticity behavior for an axis of the scrollview.

enum FindBarPosition

These constants define the position of the find bar in relation to the scroll view.

### Notifications

class let willStartLiveMagnifyNotification: NSNotification.Name

Posted at the beginning of a magnify gesture.

class let didEndLiveMagnifyNotification: NSNotification.Name

Posted at the end of a magnify gesture.

class let willStartLiveScrollNotification: NSNotification.Name

Posted on the main thread at the beginning of user-initiated live scroll tracking (gesture scroll or scroller tracking, for example, thumb dragging).

class let didLiveScrollNotification: NSNotification.Name

Posted on the main thread after changing the clipview bounds origin due to a user-initiated event.

class let didEndLiveScrollNotification: NSNotification.Name

Posted on the main thread at the end of live scroll tracking.

### Initializers

init?(coder: NSCoder)

init(frame: NSRect)

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
- NSTextFinderBarContainer
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Views

class NSScroller

An object that controls scrolling of a document view within a scroll view or other type of container view.

class NSClipView

An object that clips a document view to a scroll view’s frame.

