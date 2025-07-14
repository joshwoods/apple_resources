

- AppKit
- NSLayoutDimension
-  constraint(lessThanOrEqualTo:multiplier:constant:) 

Instance Method

# constraint(lessThanOrEqualTo:multiplier:constant:)

Returns a constraint that defines the anchor’s size attribute as greater than or equal to the specified anchor multiplied by the constant plus an offset.

macOS 10.11+

``` source
func constraint(
    lessThanOrEqualTo anchor: NSLayoutDimension,
    multiplier m: CGFloat,
    constant c: CGFloat
) -> NSLayoutConstraint
```

## Parameters 

`anchor`  

A dimension anchor from an NSView or NSLayoutGuide object.

`m`  

The multiplier constant for the constraint.

`c`  

The constant offset for this relationship.

## Return Value

An NSLayoutConstraint object that defines the attribute represented by this layout anchor as less than or equal to the attribute represented by the `anchor` parameter multiplied by the `m` constant plus the constant `c`.

## Discussion

This method defines the relationship `first attribute 

- Swift
- Objective-C

```
// Creating a constraint using NSLayoutConstraint
NSLayoutConstraint(item: button,
                   attribute: .Width,
                   relatedBy: .LessThanOrEqual,
                   toItem: button,
                   attribute: .Height,
                   multiplier: 2.0,
                   constant: 40.0).isActive = true

// Creating the same constraint using constraintLessThanOrEqualToAnchor:multiplier:constant:
button.widthAnchor.constraintLessThanOrEqualToAnchor(button.heightAnchor, multiplier: 2.0, constant: 40.0).isActive = true
```

```
// Creating a constraint using NSLayoutConstraint
[NSLayoutConstraint
 constraintWithItem:self.button
 attribute:NSLayoutAttributeWidth
 relatedBy:NSLayoutRelationLessThanOrEqual
 toItem:self.button
 attribute:NSLayoutAttributeHeight
 multiplier:2.0
 constant:40.0].active = YES;

// Creating the same constraint using constraintLessThanOrEqualToAnchor:multiplier:constant:
[self.button.widthAnchor constraintLessThanOrEqualToAnchor:self.button.heightAnchor multiplier:2.0 constant: 40.0].active = YES;
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

func constraint(lessThanOrEqualToConstant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the maximum size for the anchor’s size attribute.

