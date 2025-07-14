

- UIKit
-  NSLayoutConstraint 

Class

# NSLayoutConstraint

The relationship between two user interface objects that must be satisfied by the constraint-based layout system.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class NSLayoutConstraint
```

## Overview

Each constraint is a linear equation with the following format:

```
item1.attribute1 = multiplier × item2.attribute2 + constant
```

In this equation, `attribute1` and `attribute2` are the variables that Auto Layout can adjust when solving these constraints. The other values are defined when you create the constraint. For example, If you’re defining the relative position of two buttons, you might say “the leading edge of the second button should be 8 points after the trailing edge of the first button.” The linear equation for this relationship is shown below:

```
// positive values move to the right in left-to-right languages like English.
button2.leading = 1.0 × button1.trailing + 8.0
```

Auto Layout then modifies the values of the specified leading and trailing edges until both sides of the equation are equal. Note that Auto Layout does not simply assign the value of the right side of this equation to the left side. Instead, the system can modify either attribute or both attributes as needed to solve for this constraint.

The fact that constraints are equations (and not assignment operators) means that you can switch the order of the items in the equation as needed to more clearly express the desired relationship. However, if you switch the order, you must also invert the multiplier and constant. For example, the following two equations produce identical constraints:

```
// These equations produce identical constraints
button2.leading = 1.0 × button1.trailing + 8.0
button1.trailing = 1.0 × button2.leading - 8.0
```

A valid layout is defined as a set constraints with one and only one possible solution. Valid layouts are also referred to as a nonambiguous, nonconflicting layouts. Constraints with more than one solution are ambiguous. Constraints with no valid solutions are conflicting. For more information on resolving ambiguous and conflicting constraints, see Types of Errors in Auto Layout Guide.

Additionally, constraints are not limited to equality relationships. They can also use greater than or equal to (\>=) or less than or equal to (\Stack Views in Auto Layout Guide.

## Topics

### Creating constraints

class func constraints(withVisualFormat: String, options: NSLayoutConstraint.FormatOptions, metrics: [String : Any]?, views: [String : Any]) -> [NSLayoutConstraint]

Creates constraints described by an ASCII art-like visual format string.

convenience init(item: Any, attribute: NSLayoutConstraint.Attribute, relatedBy: NSLayoutConstraint.Relation, toItem: Any?, attribute: NSLayoutConstraint.Attribute, multiplier: CGFloat, constant: CGFloat)

Creates a constraint that defines the relationship between the specified attributes of the given views.

### Activating and deactivating constraints

var isActive: Bool

The active state of the constraint.

class func activate([NSLayoutConstraint])

Activates each constraint in the specified array.

class func deactivate([NSLayoutConstraint])

Deactivates each constraint in the specified array.

### Accessing constraint data

var firstItem: AnyObject?

The first object participating in the constraint.

var firstAttribute: NSLayoutConstraint.Attribute

The attribute of the first object participating in the constraint.

var relation: NSLayoutConstraint.Relation

The relation between the two attributes in the constraint.

var secondItem: AnyObject?

The second object participating in the constraint.

var secondAttribute: NSLayoutConstraint.Attribute

The attribute of the second object participating in the constraint.

var multiplier: CGFloat

The multiplier applied to the second attribute participating in the constraint.

var constant: CGFloat

The constant added to the multiplied second attribute participating in the constraint.

var firstAnchor: NSLayoutAnchor&lt;AnyObject>

The first anchor that defines the constraint.

var secondAnchor: NSLayoutAnchor&lt;AnyObject>?

The second anchor that defines the constraint.

### Getting the layout priority

var priority: UILayoutPriority

The priority of the constraint.

struct UILayoutPriority

The layout priority is used to indicate to the constraint-based layout system which constraints are more important, allowing the system to make appropriate tradeoffs when satisfying the constraints of the system as a whole.

struct Priority

Layout priority used to indicate the relative importance of constraints, allowing Auto Layout to make appropriate tradeoffs when satisfying the constraints of the system as a whole.

### Identifying a constraint

var identifier: String?

The name that identifies the constraint.

### Controlling constraint archiving

var shouldBeArchived: Bool

A Boolean value that determines whether the constraint should be archived by its owning view.

### Constants

enum Relation

The relation between the first attribute and the modified second attribute in a constraint.

enum Attribute

The part of the object’s visual representation that should be used to get the value for the constraint.

struct FormatOptions

A bit mask that specifies both a part of an interface element to align and a direction for the alignment between two interface elements.

enum Orientation

The layout constraint orientation, either horizontal or vertical, that the constraint uses to enforce layout between objects.

enum Axis

Keys that specify a horizontal or vertical layout constraint between objects.

struct NSEdgeInsets

A description of the distance between the edges of two rectangles.

var NSLAYOUTCONSTRAINT_H: Int32

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Constraints

Positioning content within layout margins

Position views so that they aren’t crowded by other content.

Positioning content relative to the safe area

Position views so that they aren’t obstructed by other content.

protocol UILayoutSupport

A set of methods that provide layout support and access to layout anchors.

