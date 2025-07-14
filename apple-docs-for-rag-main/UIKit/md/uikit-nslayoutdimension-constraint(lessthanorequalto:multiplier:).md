

- UIKit
- NSLayoutDimension
-  constraint(lessThanOrEqualTo:multiplier:) 

Instance Method

# constraint(lessThanOrEqualTo:multiplier:)

Returns a constraint that defines the anchor’s size attribute as less than or equal to the specified anchor multiplied by the constant.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func constraint(
    lessThanOrEqualTo anchor: NSLayoutDimension,
    multiplier m: CGFloat
) -> NSLayoutConstraint
```

## Parameters 

`anchor`  

A dimension anchor from a UIView, NSView, or UILayoutGuide object.

`m`  

The multiplier constant for the constraint.

## Return Value

An NSLayoutConstraint object that defines the attribute represented by this layout anchor as less than or equal to the attribute represented by the `anchor` parameter multiplied by the `m` constant.

## Discussion

This method defines the relationship `first attribute 

- Swift
- Objective-C

```
// Creating a constraint using NSLayoutConstraint
NSLayoutConstraint(item: saveButton,
                   attribute: .Width,
                   relatedBy: .LessThanOrEqual,
                   toItem: cancelButton,
                   attribute: .Width,
                   multiplier: 2.0,
                   constant: 0.0).isActive = true

// Creating the same constraint using constraintLessThanOrEqualToAnchor:multiplier:
saveButton.widthAnchor.constraintLessThanOrEqualToAnchor(cancelButton.widthAnchor, multiplier: 2.0).isActive = true
```

```
// Creating a constraint using NSLayoutConstraint
[NSLayoutConstraint
 constraintWithItem:self.saveButton
 attribute:NSLayoutAttributeWidth
 relatedBy:NSLayoutRelationLessThanOrEqual
 toItem:self.cancelButton
 attribute:NSLayoutAttributeWidth
 multiplier:2.0
 constant:0.0].active = YES;

// Creating the same constraint using constraintLessThanOrEqualToAnchor:multiplier:
[self.saveButton.widthAnchor constraintLessThanOrEqualToAnchor:self.cancelButton.widthAnchor multiplier:2.0].active = YES;
```

## See Also

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

func constraint(lessThanOrEqualTo: NSLayoutDimension, multiplier: CGFloat, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the anchor’s size attribute as greater than or equal to the specified anchor multiplied by the constant plus an offset.

func constraint(lessThanOrEqualToConstant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the maximum size for the anchor’s size attribute.

