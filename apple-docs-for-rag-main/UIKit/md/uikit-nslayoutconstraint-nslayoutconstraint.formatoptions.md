

- UIKit
- NSLayoutConstraint
-  NSLayoutConstraint.FormatOptions 

Structure

# NSLayoutConstraint.FormatOptions

A bit mask that specifies both a part of an interface element to align and a direction for the alignment between two interface elements.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct FormatOptions
```

## Topics

### Constants

static var alignAllLeft: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.left on each.

static var alignAllRight: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.right on each.

static var alignAllTop: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.top on each.

static var alignAllBottom: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.bottom on each.

static var alignAllLeading: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.leading on each.

static var alignAllTrailing: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.trailing on each.

static var alignAllCenterX: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.centerX on each.

static var alignAllCenterY: NSLayoutConstraint.FormatOptions

Align all specified interface elements using NSLayoutConstraint.Attribute.centerY on each.

static var alignAllLastBaseline: NSLayoutConstraint.FormatOptions

Align all specified interface elements using the last baseline of each one.

static var alignAllFirstBaseline: NSLayoutConstraint.FormatOptions

Align all specified interface elements using the first baseline of each one.

static var alignmentMask: NSLayoutConstraint.FormatOptions

Bit mask that can be combined with a NSLayoutConstraint.FormatOptions variable to yield only the alignment portion of the format options.

static var directionLeadingToTrailing: NSLayoutConstraint.FormatOptions

Arrange objects in order based on the normal text flow for the current user interface language. In left-to-right languages (like English), this arrangement results in the first object being placed farthest to the left, the next one to its right, and so on. In right-to-left languages (like Arabic or Hebrew), the ordering is reversed.

static var directionLeftToRight: NSLayoutConstraint.FormatOptions

Arrange objects in order from left to right.

static var directionRightToLeft: NSLayoutConstraint.FormatOptions

Arrange objects in order from right to left.

static var directionMask: NSLayoutConstraint.FormatOptions

A bit mask that can be combined with an NSLayoutConstraint.FormatOptions variable to yield only the direction portion of the format options.

static var spacingBaselineToBaseline: NSLayoutConstraint.FormatOptions

Align elements vertically according to their baseline positions.

static var spacingMask: NSLayoutConstraint.FormatOptions

A bit mask that can be combined with an NSLayoutConstraint.FormatOptions variable to yield only the spacing baseline spacing portion of the format options.

### Initializers

init(rawValue: UInt)

Creates a formatting-options structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

enum Relation

The relation between the first attribute and the modified second attribute in a constraint.

enum Attribute

The part of the object’s visual representation that should be used to get the value for the constraint.

enum Orientation

The layout constraint orientation, either horizontal or vertical, that the constraint uses to enforce layout between objects.

enum Axis

Keys that specify a horizontal or vertical layout constraint between objects.

struct NSEdgeInsets

A description of the distance between the edges of two rectangles.

var NSLAYOUTCONSTRAINT_H: Int32

