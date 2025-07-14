

- AppKit
- NSLayoutConstraint
-  NSLayoutConstraint.Relation 

Enumeration

# NSLayoutConstraint.Relation

The relation between the first attribute and the modified second attribute in a constraint.

macOS

``` source
enum Relation
```

## Topics

### Constants

case lessThanOrEqual

The constraint requires the first attribute to be less than or equal to the modified second attribute.

case equal

The constraint requires the first attribute to be exactly equal to the modified second attribute.

case greaterThanOrEqual

The constraint requires the first attribute to be greater than or equal to the modified second attribute.

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

enum Attribute

The part of the object’s visual representation that should be used to get the value for the constraint.

struct FormatOptions

A bit mask that specifies both a part of an interface element to align and a direction for the alignment between two interface elements.

enum Orientation

The layout constraint orientation, either horizontal or vertical, that the constraint uses to enforce layout between objects.

struct NSEdgeInsets

A description of the distance between the edges of two rectangles.

