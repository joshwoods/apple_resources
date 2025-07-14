

- AppKit
-  NSRulerView 

Class

# NSRulerView

A ruler and the markers above or to the side of a scroll view’s document view.

macOS

``` source
@MainActor
class NSRulerView
```

## Overview

Views within the scroll view can become clients of the ruler view, having it display markers for their elements, and receiving messages from the ruler view when the user manipulates the markers.

### Principal Attributes

- Displays markers that represent elements of the client view.

- Displays in arbitrary units.

- Provides for an accessory view containing extra controls.

### Creation

- hasHorizontalRuler (`NSScrollView`)

- hasVerticalRuler (`NSScrollView`)

- init(scrollView:orientation:) Designated initializer.

### Commonly Used Methods

clientView  
Changes the ruler’s client view.

markers  
Sets the markers displayed by the ruler view.

accessoryView  
Sets the accessory view.

trackMarker(_:withMouseEvent:)  
Allows the user to add a new marker.

### Overview

See NSRulerMarkerClientViewDelegation for delegate methods that may be of interest.

## Topics

### Creating a Ruler View

init(scrollView: NSScrollView?, orientation: NSRulerView.Orientation)

Initializes a newly allocated NSRulerView to have `orientation` (`NSHorizontalRuler` or `NSVerticalRuler`) within `aScrollView`.

init(coder: NSCoder)

### Altering measurement units

class func registerUnit(withName: NSRulerView.UnitName, abbreviation: String, unitToPointsConversionFactor: CGFloat, stepUpCycle: [NSNumber], stepDownCycle: [NSNumber])

Registers a new unit of measurement with the NSRulerView class, making it available to all instances of NSRulerView.

var measurementUnits: NSRulerView.UnitName

The measurement units used by the ruler to `unitName`.

struct UnitName

### Setting the client view

var clientView: NSView?

The receiver’s client view, if it has one.

### Setting an accessory view

var accessoryView: NSView?

The receiver’s accessory view to `aView`.

### Setting the zero mark position

var originOffset: CGFloat

The distance to the zero hash mark from the bounds origin of the NSScrollView’s document view (not of the receiver’s client view), in the document view’s coordinate system.

### Adding and removing markers

var markers: [NSRulerMarker]?

The receiver’s ruler markers to `markers`, removing any existing ruler markers and not consulting with the client view about the new markers.

func addMarker(NSRulerMarker)

Adds `aMarker` to the receiver, without consulting the client view for approval.

func removeMarker(NSRulerMarker)

Removes `aMarker` from the receiver, without consulting the client view for approval.

func trackMarker(NSRulerMarker, withMouseEvent: NSEvent) -> Bool

Tracks the mouse to add `aMarker` based on the initial mouse-down or mouse-dragged event `theEvent`.

### Drawing temporary ruler lines

func moveRulerline(fromLocation: CGFloat, toLocation: CGFloat)

Draws temporary lines in the ruler area.

### Drawing

func drawHashMarksAndLabels(in: NSRect)

Draws the receiver’s hash marks and labels in `aRect`, which is expressed in the receiver’s coordinate system.

func drawMarkers(in: NSRect)

Draws the receiver’s markers in `aRect`, which is expressed in the receiver’s coordinate system.

func invalidateHashMarks()

Forces recalculation of the hash mark spacing for the next time the receiver is displayed.

### Ruler layout

var scrollView: NSScrollView?

The NSScrollView that owns the receiver to `scrollView`, without retaining it.

var orientation: NSRulerView.Orientation

The orientation of the receiver to `orientation`.

enum Orientation

These constants are defined to specify a ruler’s orientation and are used by orientation.

var reservedThicknessForAccessoryView: CGFloat

The room available for the receiver’s accessory view to `thickness`.

var reservedThicknessForMarkers: CGFloat

The room available for ruler markers to `thickness`.

var ruleThickness: CGFloat

The thickness of the area where ruler hash marks and labels are drawn.

var requiredThickness: CGFloat

The thickness needed for proper tiling of the receiver within an NSScrollView.

var baselineLocation: CGFloat

The location of the receiver’s baseline, in its own coordinate system.

var isFlipped: Bool

A Boolean that indicates if the ruler view’s coordinate system is flipped.

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

### Rulers

class NSRulerMarker

A symbol on a ruler view, indicating a location for the graphics element it represents in the client of the ruler view.

