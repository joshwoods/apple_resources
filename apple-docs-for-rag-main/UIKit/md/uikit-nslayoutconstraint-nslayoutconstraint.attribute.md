

- UIKit
- NSLayoutConstraint
-  NSLayoutConstraint.Attribute 

Enumeration

# NSLayoutConstraint.Attribute

The part of the object’s visual representation that should be used to get the value for the constraint.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum Attribute
```

## Topics

### Constants

case left

The left side of the object’s alignment rectangle.

case right

The right side of the object’s alignment rectangle.

case top

The top of the object’s alignment rectangle.

case bottom

The bottom of the object’s alignment rectangle.

case leading

The leading edge of the object’s alignment rectangle.

case trailing

The trailing edge of the object’s alignment rectangle.

case width

The width of the object’s alignment rectangle.

case height

The height of the object’s alignment rectangle.

case centerX

The center along the x-axis of the object’s alignment rectangle.

case centerY

The center along the y-axis of the object’s alignment rectangle.

case lastBaseline

The object’s baseline.

case firstBaseline

The object’s baseline.

case leftMargin

The object’s left margin.

case rightMargin

The object’s right margin.

case topMargin

The object’s top margin.

case bottomMargin

The object’s bottom margin.

case leadingMargin

The object’s leading margin.

case trailingMargin

The object’s trailing margin.

case centerXWithinMargins

The center along the x-axis between the object’s left and right margin.

case centerYWithinMargins

The center along the y-axis between the object’s top and bottom margin.

case notAnAttribute

A placeholder value for indicating that the constraint’s second item and second attribute aren’t used in any calculations.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum Relation

The relation between the first attribute and the modified second attribute in a constraint.

struct FormatOptions

A bit mask that specifies both a part of an interface element to align and a direction for the alignment between two interface elements.

enum Orientation

The layout constraint orientation, either horizontal or vertical, that the constraint uses to enforce layout between objects.

enum Axis

Keys that specify a horizontal or vertical layout constraint between objects.

struct NSEdgeInsets

A description of the distance between the edges of two rectangles.

var NSLAYOUTCONSTRAINT_H: Int32

