

- AppKit
-  NSScroller 

Class

# NSScroller

An object that controls scrolling of a document view within a scroll view or other type of container view.

macOS

``` source
@MainActor
class NSScroller
```

## Overview

A scroller displays a slot containing a knob that the user can drag directly to the desired location. The knob indicates both the position within the document view and—by varying in size within the slot—the amount visible relative to the size of the document view.

Typically, you don’t need to program with scrollers; instead, you configure them with an NSScrollView object in a Nib file.

Don’t use an scroller when a slider would be more appropriate. An NSSlider object represents a range of values for something in the application and lets the user choose a setting. A scroller represents the relative position of the visible portion of a view and lets the user choose which portion to view.

## Topics

### Determining Scroller Size

class func scrollerWidth(for: NSControl.ControlSize, scrollerStyle: NSScroller.Style) -> CGFloat

Returns the width for scrollers of the receiving class for a given control size and scroller style.

var controlSize: NSControl.ControlSize

The size of the scroller.

### Laying out a Scroller

var arrowsPosition: NSScroller.ArrowPosition

The location of the scroll buttons within the scroller, as described in NSScroller.ArrowPosition.

Deprecated

### Setting the Knob Position

var knobProportion: CGFloat

The proportion of the knob slot that the knob should fill.

### Calculating Layout

func rect(for: NSScroller.Part) -> NSRect

Returns the rectangle occupied by `aPart`, which for this method is interpreted literally rather than as an indicator of scrolling direction.

func testPart(NSPoint) -> NSScroller.Part

Returns the part that would be hit by a mouse-down event at `aPoint` (expressed in the window’s coordinate system).

func checkSpaceForParts()

Checks to see if there is enough room in the receiver to display the knob and buttons.

var usableParts: NSScroller.UsableParts

A value that indicates which parts of the receiver are displayed and usable.

### Drawing Scroller Parts

func drawArrow(NSScroller.Arrow, highlight: Bool)

Draws the scroll button indicated by `arrow`, which is either `NSScrollerIncrementArrow` (the down or right scroll button) or `NSScrollerDecrementArrow` (up or left).

Deprecated

func drawKnobSlot(in: NSRect, highlight: Bool)

Draws the portion of the scroller’s track, possibly including the line increment and decrement arrow buttons, that falls in the given rectangle.

func drawKnob()

Draws the knob.

func highlight(Bool)

Highlights or unhighlights the scroll button the user clicked.

Deprecated

### Event Handling

var hitPart: NSScroller.Part

A part code indicating the manner in which the scrolling should be performed.

func trackKnob(with: NSEvent)

Tracks the knob and sends action messages to the receiver’s target.

func trackScrollButtons(with: NSEvent)

Tracks the scroll buttons and sends action messages to the receiver’s target.

Deprecated

### Setting Control Tint

var controlTint: NSControlTint

The scroller’s control tint.

Deprecated

### Managing Presentation Style

class var preferredScrollerStyle: NSScroller.Style

Returns the style of scrollers that applications should use wherever possible.

var scrollerStyle: NSScroller.Style

The scroller style for this scroller.

var knobStyle: NSScroller.KnobStyle

The scroller’s knob style.

### Constants

enum Style

Constants to specify the scroller style.

enum KnobStyle

Specify different knob styles.

enum Part

These constants specify the different parts of the scroller:

enum Arrow

These constants describe the two scroller buttons and are used by drawArrow(_:highlight:).

Deprecated

enum ArrowPosition

These constants specify where the scroller’s buttons appear and are used by the arrowsPosition property.

Deprecated

enum UsableParts

These constants specify which parts of the scroller are visible.

### Notifications

class let preferredScrollerStyleDidChangeNotification: NSNotification.Name

Posted if the preferred scroller style changes.

### Instance Properties

var knobProportion: CGFloat

The proportion of the knob slot that the knob should fill.

### Type Properties

class var isCompatibleWithOverlayScrollers: Bool

## Relationships

### Inherits From

- NSControl

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

class NSClipView

An object that clips a document view to a scroll view’s frame.

