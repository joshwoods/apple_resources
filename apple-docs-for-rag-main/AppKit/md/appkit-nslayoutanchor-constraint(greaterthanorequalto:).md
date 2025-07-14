

- AppKit
- NSLayoutAnchor
-  constraint(greaterThanOrEqualTo:) 

Instance Method

# constraint(greaterThanOrEqualTo:)

Returns a constraint that defines one item’s attribute as greater than or equal to another.

macOS 10.11+

``` source
func constraint(greaterThanOrEqualTo anchor: NSLayoutAnchor) -> NSLayoutConstraint
```

## Parameters 

`anchor`  

A layout anchor from an NSView or NSLayoutGuide object. You must use a subclass of NSLayoutAnchor that matches the current anchor. For example, if you call this method on an NSLayoutXAxisAnchor object, this parameter must be another NSLayoutXAxisAnchor.

## Return Value

An NSLayoutConstraint object that defines the attribute represented by this layout anchor as greater than or equal to the attribute represented by the `anchor` parameter.

## Discussion

This method creates a relationship where `first attribute >= second attribute`. Where `first attribute` is the layout attribute represented by the anchor receiving this method call, and `second attribute` is the layout attribute represented by the `anchor` parameter. All values are measured in points; however, these values can be interpreted in different ways, depending on the type of layout anchor.

- For leading or trailing anchors, the values increase as you move in the current language’s reading direction. In English, for example, values increase as you move to the right.

- For left and right anchors, the values increase as you move to the right.

- For NSLayoutYAxisAnchor objects, the values increase as you move down.

- For NSLayoutDimension objects, the values increase as the items increase in size.

The constraints produced by the following two examples are identical.

- Swift
- Objective-C

```
// Creating a constraint using NSLayoutConstraint
NSLayoutConstraint(item: subview,
                   attribute: .Leading,
                   relatedBy: .GreaterThanOrEqual,
                   toItem: view,
                   attribute: .LeadingMargin,
                   multiplier: 1.0,
                   constant: 0.0).isActive = true

// Creating the same constraint using constraintGreaterThanOrEqualToAnchor:
let margins = view.layoutMarginsGuide
subview.leadingAnchor.constraintGreaterThanOrEqualToAnchor(margins.leadingAnchor).isActive = true
```

```
// Creating a constraint using NSLayoutConstraint
[NSLayoutConstraint
 constraintWithItem:subview
 attribute:NSLayoutAttributeLeading
 relatedBy:NSLayoutRelationGreaterThanOrEqual
 toItem:self.view
 attribute:NSLayoutAttributeLeadingMargin
 multiplier:1.0
 constant:0.0].active = YES;

// Creating the same constraint using constraintGreaterThanOrEqualToAnchor:
NSLayoutGuide *margin = self.view.layoutMarginsGuide;
[subview.leadingAnchor constraintGreaterThanOrEqualToAnchor:margin.leadingAnchor].active = YES;
```

## See Also

### Building constraints

func constraint(equalTo: NSLayoutAnchor&lt;AnchorType>) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as equal to another.

func constraint(equalTo: NSLayoutAnchor&lt;AnchorType>, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as equal to another item’s attribute plus a constant offset.

func constraint(greaterThanOrEqualTo: NSLayoutAnchor&lt;AnchorType>, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as greater than or equal to another item’s attribute plus a constant offset.

func constraint(lessThanOrEqualTo: NSLayoutAnchor&lt;AnchorType>) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as less than or equal to another.

func constraint(lessThanOrEqualTo: NSLayoutAnchor&lt;AnchorType>, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines one item’s attribute as less than or equal to another item’s attribute plus a constant offset.

