

- AppKit
- NSLayoutDimension
-  constraint(greaterThanOrEqualTo:multiplier:constant:) 

Instance Method

# constraint(greaterThanOrEqualTo:multiplier:constant:)

Returns a constraint that defines the anchor’s size attribute as greater than or equal to the specified anchor multiplied by the constant plus an offset.

macOS 10.11+

``` source
func constraint(
    greaterThanOrEqualTo anchor: NSLayoutDimension,
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

An NSLayoutConstraint object that defines the attribute represented by this layout anchor as greater than or equal to the attribute represented by the `anchor` parameter multiplied by the `m` constant plus the constant `c`.

## Discussion

This method defines the relationship `first attribute >= (m * second attribute) + c`. Where `first attribute` is the layout attribute represented by the anchor receiving this method call, and `second attribute` is the layout attribute represented by the `anchor` parameter.

The constraints produced by the following two examples are identical.

- Swift
- Objective-C

```
// Creating a constraint using NSLayoutConstraint
NSLayoutConstraint(item: button,
                   attribute: .Width,
                   relatedBy: .GreaterThanOrEqual,
                   toItem: button,
                   attribute: .Height,
                   multiplier: 2.0,
                   constant: 40.0).isActive = true

// Creating the same constraint using constraintGreaterThanOrEqualToAnchor:multiplier:constant:
button.widthAnchor.constraintGreaterThanOrEqualToAnchor(button.heightAnchor, multiplier: 2.0, constant: 40.0).isActive = true
```

```
// Creating a constraint using NSLayoutConstraint
[NSLayoutConstraint
 constraintWithItem:self.button
 attribute:NSLayoutAttributeWidth
 relatedBy:NSLayoutRelationGreaterThanOrEqual
 toItem:self.button
 attribute:NSLayoutAttributeHeight
 multiplier:2.0
 constant:40.0].active = YES;

// Creating the same constraint using constraintGreaterThanOrEqualToAnchor:multiplier:constant:
[self.button.widthAnchor constraintGreaterThanOrEqualToAnchor:self.button.heightAnchor multiplier:2.0 constant: 40.0].active = YES;
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

func constraint(greaterThanOrEqualToConstant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the minimum size for the anchor’s size attribute.

func constraint(lessThanOrEqualTo: NSLayoutDimension, multiplier: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the anchor’s size attribute as less than or equal to the specified anchor multiplied by the constant.

func constraint(lessThanOrEqualTo: NSLayoutDimension, multiplier: CGFloat, constant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the anchor’s size attribute as greater than or equal to the specified anchor multiplied by the constant plus an offset.

func constraint(lessThanOrEqualToConstant: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the maximum size for the anchor’s size attribute.

