

- AppKit
-  NSLayoutAnchor 

Class

# NSLayoutAnchor

A factory class for creating layout constraint objects using a fluent API.

macOS 10.11+

``` source
class NSLayoutAnchor where AnchorType : AnyObject
```

## Overview

Use these constraints to programatically define your layout using Auto Layout. Instead of creating NSLayoutConstraint objects directly, start with an NSView or NSLayoutGuide object you wish to constrain, and select one of that object’s anchor properties. These properties correspond to the main NSLayoutConstraint.Attribute values used in Auto Layout, and provide an appropriate NSLayoutAnchor subclass for creating constraints to that attribute. Use the anchor’s methods to construct your constraint.

- Swift
- Objective-C

```
// Creating constraints using NSLayoutConstraint
NSLayoutConstraint(item: subview,
                   attribute: .leading,
                   relatedBy: .equal,
                   toItem: view,
                   attribute: .leadingMargin,
                   multiplier: 1.0,
                   constant: 0.0).isActive = true

NSLayoutConstraint(item: subview,
                   attribute: .trailing,
                   relatedBy: .equal,
                   toItem: view,
                   attribute: .trailingMargin,
                   multiplier: 1.0,
                   constant: 0.0).isActive = true

// Creating the same constraints using Layout Anchors
let margins = view.layoutMarginsGuide

subview.leadingAnchor.constraint(equalTo: margins.leadingAnchor).isActive = true
subview.trailingAnchor.constraint(equalTo: margins.trailingAnchor).isActive = true

```

```
// Creating constraints using NSLayoutConstraint
[NSLayoutConstraint
 constraintWithItem:subview
 attribute:NSLayoutAttributeLeading
 relatedBy:NSLayoutRelationEqual
 toItem:self.view
 attribute:NSLayoutAttributeLeadingMargin
 multiplier:1.0
 constant:0.0].active = YES;

[NSLayoutConstraint
 constraintWithItem:subview
 attribute:NSLayoutAttributeTrailing
 relatedBy:NSLayoutRelationEqual
 toItem:self.view
 attribute:NSLayoutAttributeTrailingMargin
 multiplier:1.0
 constant:0.0].active = YES;

// Creating the same constraints using Layout Anchors
NSLayoutGuide *margin = self.view.layoutMarginsGuide;

[subview.leadingAnchor constraintEqualToAnchor:margin.leadingAnchor].active = YES;
[subview.trailingAnchor constraintEqualToAnchor:margin.trailingAnchor].active = YES;
```

As you can see from these examples, the NSLayoutAnchor class provides several advantages over using the NSLayoutConstraint API directly.

- The code is cleaner, more concise, and easier to read.

- The NSLayoutConstraint.Attribute subclasses provide additional type checking, preventing you from creating invalid constraints.

Note

While the NSLayoutAnchor class provides additional type checking, it is still possible to create invalid constraints. For example, the compiler allows you to constrain one view’s leadingAnchor with another view’s leftAnchor, since they are both NSLayoutXAxisAnchor instances. However, Auto Layout does not allow constraints that mix leading and trailing attributes with left or right attributes. As a result, this constraint crashes at runtime.

For more information on the anchor properties, see bottomAnchor in the NSView or NSLayoutGuide.

Note

You never use the NSLayoutAnchor class directly. Instead, use one of its subclasses, based on the type of constraint you wish to create.

- Use NSLayoutXAxisAnchor to create horizontal constraints.

- Use NSLayoutYAxisAnchor to create vertical constraints.

- Use NSLayoutDimension to create constraints that affect the view’s height or width.

However, since you access NSLayoutAnchor objects using the anchor properties of an NSView or NSLayoutGuide, a correct subclass is automatically provided.

## Topics

### Building constraints

func constraint(equalTo: NSLayoutAnchor&lt;AnchorType>) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as equal to another.

func constraint(equalTo: NSLayoutAnchor&lt;AnchorType>, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as equal to another item’s attribute plus a constant offset.

func constraint(greaterThanOrEqualTo: NSLayoutAnchor&lt;AnchorType>) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as greater than or equal to another.

func constraint(greaterThanOrEqualTo: NSLayoutAnchor&lt;AnchorType>, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as greater than or equal to another item’s attribute plus a constant offset.

func constraint(lessThanOrEqualTo: NSLayoutAnchor&lt;AnchorType>) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as less than or equal to another.

func constraint(lessThanOrEqualTo: NSLayoutAnchor&lt;AnchorType>, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as less than or equal to another item’s attribute plus a constant offset.

### Debugging the anchor

var constraintsAffectingLayout: [NSLayoutConstraint]

The constraints that impact the layout of the anchor.

var hasAmbiguousLayout: Bool

A Boolean value indicating whether the constraints impacting the anchor specify its location ambiguously.

var name: String

The name assigned to the anchor for debugging purposes.

var item: AnyObject?

The layout item used to calculate the anchor’s position.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSLayoutDimension
- NSLayoutXAxisAnchor
- NSLayoutYAxisAnchor

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

### Anchors

class NSLayoutXAxisAnchor

A factory class for creating horizontal layout constraint objects using a fluent API.

class NSLayoutYAxisAnchor

A factory class for creating vertical layout constraint objects using a fluent API.

