

- UIKit
- NSLayoutAnchor
-  constraint(lessThanOrEqualTo:) 

Instance Method

# constraint(lessThanOrEqualTo:)

Returns a constraint that defines one item’s attribute as less than or equal to another.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func constraint(lessThanOrEqualTo anchor: NSLayoutAnchor) -> NSLayoutConstraint
```

## Parameters 

`anchor`  

A layout anchor from a UIView, NSView, or UILayoutGuide object. You must use a subclass of NSLayoutAnchor that matches the current anchor. For example, if you call this method on an NSLayoutXAxisAnchor object, this parameter must be another NSLayoutXAxisAnchor.

## Return Value

An NSLayoutConstraint object that defines the attribute represented by this layout anchor as less than or equal to the attribute represented by the `anchor` parameter.

## Discussion

This method defines the relationship `first attribute NSLayoutYAxisAnchor objects, the values increase as you move down.

- For NSLayoutDimension objects, the values increase as the items increase in size.

The constraints produced by the following two examples are identical.

- Swift
- Objective-C

```
// Creating a constraint using NSLayoutConstraint
NSLayoutConstraint(item: subview,
                   attribute: .Leading,
                   relatedBy: .LessThanOrEqual,
                   toItem: view,
                   attribute: .LeadingMargin,
                   multiplier: 1.0,
                   constant: 0.0).isActive = true

// Creating the same constraint using constraintLessThanOrEqualToAnchor:
let margins = view.layoutMarginsGuide
subview.leadingAnchor.constraintLessThanOrEqualToAnchor(margins.leadingAnchor).isActive = true
```

```
// Creating a constraint using NSLayoutConstraint
[NSLayoutConstraint
 constraintWithItem:subview
 attribute:NSLayoutAttributeLeading
 relatedBy:NSLayoutRelationLessThanOrEqual
 toItem:self.view
 attribute:NSLayoutAttributeLeadingMargin
 multiplier:1.0
 constant:0.0].active = YES;

// Creating the same constraint using constraintLessThanOrEqualToAnchor:
UILayoutGuide *margin = self.view.layoutMarginsGuide;
[subview.leadingAnchor constraintLessThanOrEqualToAnchor:margin.leadingAnchor].active = YES;
```

## See Also

### Building constraints

func constraint(equalTo: NSLayoutAnchor&lt;AnchorType>) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as equal to another.

func constraint(equalTo: NSLayoutAnchor&lt;AnchorType>, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as equal to another item’s attribute plus a constant offset.

func constraint(greaterThanOrEqualTo: NSLayoutAnchor&lt;AnchorType>) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as greater than or equal to another.

func constraint(greaterThanOrEqualTo: NSLayoutAnchor&lt;AnchorType>, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as greater than or equal to another item’s attribute plus a constant offset.

func constraint(lessThanOrEqualTo: NSLayoutAnchor&lt;AnchorType>, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as less than or equal to another item’s attribute plus a constant offset.

