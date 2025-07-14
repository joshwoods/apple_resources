

- UIKit
-  NSLayoutDimension 

Class

# NSLayoutDimension

A factory class for creating size-based layout constraint objects using a fluent API.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class NSLayoutDimension
```

## Overview

Use these constraints to programmatically define your layout using Auto Layout. All sizes are measured in points. In addition to providing size-specific methods for creating constraints, this class adds type information to the methods inherited from NSLayoutAnchor. Specifically, the generic methods declared by NSLayoutAnchor must now take a matching NSLayoutDimension object.

- Swift
- Objective-C

```
// This code works as expected.
saveButton.widthAnchor.constraint(equalTo: cancelButton.widthAnchor).isActive = true

// This code generates an incompatible pointer type warning.
saveButton.widthAnchor.constraint(equalTo: cancelButton.leadingAnchor).isActive = true
```

```
// This code works as expected.
[self.saveButton.widthAnchor constraintEqualToAnchor:self.cancelButton.widthAnchor].active = YES;

// This code generates an incompatible pointer type warning.
[self.saveButton.widthAnchor constraintEqualToAnchor:self.cancelButton.leadingAnchor].active = YES;
```

For more information on using layout anchors, see NSLayoutAnchor.

## Topics

### Building constraints

func constraint(equalTo: NSLayoutDimension, multiplier: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the anchor’s size attribute as equal to the specified anchor multiplied by the constant.

func constraint(equalTo: NSLayoutDimension, multiplier: CGFloat, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the anchor’s size attribute as equal to the specified size attribute multiplied by a constant plus an offset.

func constraint(equalToConstant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines a constant size for the anchor’s size attribute.

func constraint(greaterThanOrEqualTo: NSLayoutDimension, multiplier: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the anchor’s size attribute as greater than or equal to the specified anchor multiplied by the constant.

func constraint(greaterThanOrEqualTo: NSLayoutDimension, multiplier: CGFloat, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the anchor’s size attribute as greater than or equal to the specified anchor multiplied by the constant plus an offset.

func constraint(greaterThanOrEqualToConstant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the minimum size for the anchor’s size attribute.

func constraint(lessThanOrEqualTo: NSLayoutDimension, multiplier: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the anchor’s size attribute as less than or equal to the specified anchor multiplied by the constant.

func constraint(lessThanOrEqualTo: NSLayoutDimension, multiplier: CGFloat, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the anchor’s size attribute as greater than or equal to the specified anchor multiplied by the constant plus an offset.

func constraint(lessThanOrEqualToConstant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the maximum size for the anchor’s size attribute.

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
- Sendable

## See Also

### Layout guides

class UILayoutGuide

A rectangular area that can interact with Auto Layout.

