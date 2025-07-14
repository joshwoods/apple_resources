

- AppKit
- NSLayoutAnchor
-  constraint(equalTo:) 

Instance Method

# constraint(equalTo:)

Returns a constraint that defines one item’s attribute as equal to another.

macOS 10.11+

``` source
func constraint(equalTo anchor: NSLayoutAnchor) -> NSLayoutConstraint
```

## Parameters 

`anchor`  

A layout anchor from an NSView or NSLayoutGuide object. You must use a subclass of NSLayoutAnchor that matches the current anchor. For example, if you call this method on an NSLayoutXAxisAnchor object, this parameter must be another NSLayoutXAxisAnchor.

## Return Value

An NSLayoutConstraint object that defines an equal relationship between the attributes represented by the two layout anchors.

## Discussion

This method defines the relationship `first attribute = second attribute`. Where `first attribute` is the layout attribute represented by the anchor receiving this method call, and `second attribute` is the layout attribute represented by the `anchor` parameter.

The constraints produced by the following two examples are identical.

- Swift
- Objective-C

```
// Creating a constraint using NSLayoutConstraint
NSLayoutConstraint(item: subview,
                   attribute: .Leading,
                   relatedBy: .Equal,
                   toItem: view,
                   attribute: .LeadingMargin,
                   multiplier: 1.0,
                   constant: 0.0).isActive = true

// Creating the same constraint using constraintEqualToAnchor:
let margins = view.layoutMarginsGuide
subview.leadingAnchor.constraintEqualToAnchor(margins.leadingAnchor).isActive = true
```

```
// Creating a constraint using NSLayoutConstraint
[NSLayoutConstraint
 constraintWithItem:subview
 attribute:NSLayoutAttributeLeading
 relatedBy:NSLayoutRelationEqual
 toItem:self.view
 attribute:NSLayoutAttributeLeadingMargin
 multiplier:1.0
 constant:0.0].active = YES;

// Creating the same constraint using constraintEqualToAnchor:
NSLayoutGuide *margin = self.view.layoutMarginsGuide;
[subview.leadingAnchor constraintEqualToAnchor:margin.leadingAnchor].active = YES;
```

## See Also

### Related Documentation

class NSLayoutConstraint

The relationship between two user interface objects that must be satisfied by the constraint-based layout system.

Auto Layout Guide

### Building constraints

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

