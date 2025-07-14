

- AppKit
- Views and Controls
- NSView
-  View Coordinates 

API Collection

# View Coordinates

Manage the frame and bounds rectangles that determine the size and position of the view in the view hierarchy.

## Topics

### Modifying the Frame Rectangle

var frame: NSRect

The view’s frame rectangle, which defines its position and size in its superview’s coordinate system.

func setFrameOrigin(NSPoint)

Sets the origin of the view’s frame rectangle to the specified point, effectively repositioning it within its superview.

func setFrameSize(NSSize)

Sets the size of the view’s frame rectangle to the specified dimensions, resizing it within its superview without affecting its coordinate system.

var frameRotation: CGFloat

The angle of rotation, measured in degrees, applied to the view’s frame rectangle relative to its superview’s coordinate system.

class let frameDidChangeNotification: NSNotification.Name

Posted whenever the view’s frame rectangle changes to a new value, but only when the view’s postsFrameChangedNotifications property is true.

var postsFrameChangedNotifications: Bool

A Boolean value indicating whether the view posts notifications when its frame rectangle changes.

### Modifying the Bounds Rectangle

var bounds: NSRect

The view’s bounds rectangle, which expresses its location and size in its own coordinate system.

func setBoundsOrigin(NSPoint)

Sets the origin of the view’s bounds rectangle to a specified point.

func setBoundsSize(NSSize)

Sets the size of the view’s bounds rectangle to specified dimensions, inversely scaling its coordinate system relative to its frame rectangle.

var boundsRotation: CGFloat

The angle of rotation, measured in degrees, applied to the view’s bounds rectangle relative to its frame rectangle.

class let boundsDidChangeNotification: NSNotification.Name

Posted whenever the `NSView`‘s bounds rectangle changes to a new value independently of the frame rectangle, but only when the view’s postsBoundsChangedNotifications property is true.

var postsBoundsChangedNotifications: Bool

A Boolean value indicating whether the view posts notifications when its bounds rectangle changes.

### Examining Coordinate System Modifications

var isFlipped: Bool

A Boolean value indicating whether the view uses a flipped coordinate system.

var isRotatedFromBase: Bool

A Boolean value indicating whether the view or any of its ancestors has ever had a rotation factor applied to its frame or bounds.

var isRotatedOrScaledFromBase: Bool

A Boolean value indicating whether the view or any of its ancestors has ever had a rotation factor applied to its frame or bounds, or has been scaled from the window’s base coordinate system.

### Modifying the Coordinate System

func translateOrigin(to: NSPoint)

Translates the view’s coordinate system so that its origin moves to a new location.

func scaleUnitSquare(to: NSSize)

Scales the view’s coordinate system so that the unit square scales to the specified dimensions.

func rotate(byDegrees: CGFloat)

Rotates the view’s bounds rectangle by a specified degree value around the origin of the coordinate system, (0.0, 0.0).

### Converting Coordinate Values

func backingAlignedRect(NSRect, options: AlignmentOptions) -> NSRect

Returns a backing store pixel-aligned rectangle in local view coordinates.

func convertFromBacking(NSPoint) -> NSPoint

Converts a point from its pixel aligned backing store coordinate system to the view’s interior coordinate system.

func convertToBacking(NSPoint) -> NSPoint

Converts a point from the view’s interior coordinate system to its pixel aligned backing store coordinate system.

func convertFromLayer(NSPoint) -> NSPoint

Convert the point from the layer’s interior coordinate system to the view’s interior coordinate system.

func convertToLayer(NSPoint) -> NSPoint

Convert the size from the view’s interior coordinate system to the layer’s interior coordinate system.

func convertFromBacking(NSRect) -> NSRect

Converts a rectangle from its pixel aligned backing store coordinate system to the view’s interior coordinate system.

func convertToBacking(NSRect) -> NSRect

Converts a rectangle from the view’s interior coordinate system to its pixel aligned backing store coordinate system.

func convertFromLayer(NSRect) -> NSRect

Convert the rectangle from the layer’s interior coordinate system to the view’s interior coordinate system.

func convertToLayer(NSRect) -> NSRect

Convert the size from the view’s interior coordinate system to the layer’s interior coordinate system.

func convertFromBacking(NSSize) -> NSSize

Converts a size from its pixel aligned backing store coordinate system to the view’s interior coordinate system.

func convertToBacking(NSSize) -> NSSize

Converts a size from the view’s interior coordinate system to its pixel aligned backing store coordinate system.

func convertFromLayer(NSSize) -> NSSize

Convert the size from the layer’s interior coordinate system to the view’s interior coordinate system.

func convertToLayer(NSSize) -> NSSize

Convert the size from the view’s interior coordinate system to the layer’s interior coordinate system.

func convert(NSPoint, from: NSView?) -> NSPoint

Converts a point from the coordinate system of a given view to that of the view.

func convert(NSPoint, to: NSView?) -> NSPoint

Converts a point from the view’s coordinate system to that of a given view.

func convert(NSSize, from: NSView?) -> NSSize

Converts a size from another view’s coordinate system to that of the view.

func convert(NSSize, to: NSView?) -> NSSize

Converts a size from the view’s coordinate system to that of another view.

func convert(NSRect, from: NSView?) -> NSRect

Converts a rectangle from the coordinate system of another view to that of the view.

func convert(NSRect, to: NSView?) -> NSRect

Converts a rectangle from the view’s coordinate system to that of another view.

func centerScanRect(NSRect) -> NSRect

Converts the corners of a specified rectangle to lie on the center of device pixels, which is useful in compensating for rendering overscanning when the coordinate system has been scaled.

## See Also

### Configuring the view

View Hierarchy

Manage the subviews, superview, and window of a view and respond to notifications when the view hierarchy changes.

Appearance

Change the view’s visibility, vibrancy, and focus ring and respond to appearance-related changes.

Core Animation Support

Manage the layer object that provides the view’s visual representation and accelerates drawing operations.

Related UI

Manage contextual menus, cursors, tool tips, and other system-provided windows and content.

