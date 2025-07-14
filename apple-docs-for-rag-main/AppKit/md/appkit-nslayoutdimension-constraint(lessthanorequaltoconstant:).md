

- AppKit
- NSLayoutDimension
-  constraint(lessThanOrEqualToConstant:) 

Instance Method

# constraint(lessThanOrEqualToConstant:)

Returns a constraint that defines the maximum size for the anchor’s size attribute.

macOS 10.11+

``` source
func constraint(lessThanOrEqualToConstant c: CGFloat) -> NSLayoutConstraint
```

## Parameters 

`c`  

A constant representing the maximum size of the attribute associated with this dimension anchor.

## Return Value

An NSLayoutConstraint object that defines a maximum size for the attribute associated with this dimension anchor.

## Discussion

This method defines the relationship `first attribute 

- Swift
- Objective-C

```
// Creating a constraint using NSLayoutConstraint
NSLayoutConstraint(item: button,
                   attribute: .Width,
                   relatedBy: .LessThanOrEqual,
                   toItem: nil,
                   attribute: .NotAnAttribute,
                   multiplier: 1.0,
                   constant: 40.0).isActive = true

// Creating the same constraint using constraintLessThanOrEqualToConstant:
button.widthAnchor.constraintLessThanOrEqualToConstant(40.0).isActive = true
```

```
// Creating a constraint using NSLayoutConstraint
[NSLayoutConstraint
 constraintWithItem:self.button
 attribute:NSLayoutAttributeWidth
 relatedBy:NSLayoutRelationLessThanOrEqual
 toItem:nil
 attribute:NSLayoutAttributeNotAnAttribute
 multiplier:1.0
 constant:40.0].active = YES;

// Creating the same constraint using constraintLessThanOrEqualToConstant:
[self.button.widthAnchor constraintLessThanOrEqualToConstant: 40.0].active = YES;
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

func constraint(lessThanOrEqualTo: NSLayoutDimension, multiplier: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the anchor’s size attribute as less than or equal to the specified anchor multiplied by the constant.

func constraint(lessThanOrEqualTo: NSLayoutDimension, multiplier: CGFloat, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the anchor’s size attribute as greater than or equal to the specified anchor multiplied by the constant plus an offset.

