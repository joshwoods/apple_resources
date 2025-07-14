

- AppKit
-  NSLayoutYAxisAnchor 

Class

# NSLayoutYAxisAnchor

A factory class for creating vertical layout constraint objects using a fluent API.

macOS 10.11+

``` source
class NSLayoutYAxisAnchor
```

## Overview

NSLayoutYAxisAnchor adds type information to the methods inherited from NSLayoutAnchor. Specifically, the generic methods declared by NSLayoutAnchor must now take a matching NSLayoutYAxisAnchor object.

- Swift
- Objective-C

```
// This constraint is valid
cancelButton.topAnchor.constraintEqualToAnchor(saveButton.topAnchor, constant: 8.0).isActive = true

// This constraint generates an incompatible pointer type warning
cancelButton.topAnchor.constraintEqualToAnchor(saveButton.trailingAnchor, constant: 8.0).isActive = true
```

```
// This constraint is valid
[self.cancelButton.leadingAnchor constraintEqualToAnchor:self.saveButton.trailingAnchor  constant: 8.0].active = true;

// This constraint generates an incompatible pointer type warning
[self.cancelButton.topAnchor constraintEqualToAnchor:self.saveButton.trailingAnchor constant: 8.0].active = true;
```

For more information on using layout anchors, see NSLayoutAnchor.

## Topics

### Building system spacing constraints

func constraint(equalToSystemSpacingBelow: NSLayoutYAxisAnchor, multiplier: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the specific distance at which the current anchor is positioned below the specified anchor.

func constraint(greaterThanOrEqualToSystemSpacingBelow: NSLayoutYAxisAnchor, multiplier: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the minimum distance by which the current anchor is positioned below the specified anchor.

func constraint(lessThanOrEqualToSystemSpacingBelow: NSLayoutYAxisAnchor, multiplier: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the maximum distance by which the current anchor is positioned below the specified anchor.

Creating self-sizing table view cells

Create table view cells that support Dynamic Type and use system spacing constraints to adjust the spacing surrounding text labels.

### Creating a layout dimension

func anchorWithOffset(to: NSLayoutYAxisAnchor) -> NSLayoutDimension

Creates a layout dimension object from two anchors.

## Relationships

### Inherits From

- NSLayoutAnchor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Related Documentation

class NSLayoutConstraint

The relationship between two user interface objects that must be satisfied by the constraint-based layout system.

Auto Layout Guide

### Anchors

class NSLayoutAnchor

A factory class for creating layout constraint objects using a fluent API.

class NSLayoutXAxisAnchor

A factory class for creating horizontal layout constraint objects using a fluent API.

