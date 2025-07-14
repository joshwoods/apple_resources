

- AppKit
- NSLayoutXAxisAnchor
-  constraint(greaterThanOrEqualToSystemSpacingAfter:multiplier:) 

Instance Method

# constraint(greaterThanOrEqualToSystemSpacingAfter:multiplier:)

Returns a constraint that defines the minimum amount by which the current anchor trails the specified anchor.

macOS 11.0+

``` source
func constraint(
    greaterThanOrEqualToSystemSpacingAfter anchor: NSLayoutXAxisAnchor,
    multiplier: CGFloat
) -> NSLayoutConstraint
```

## Parameters 

`anchor`  

The anchor to use as the starting point for the constraint.

`multiplier`  

The multiple of the system spacing to use as the minimum distance between the two anchors.

## Return Value

An NSLayoutConstraint object that imposes a minimum distance between the current anchor and the object in the `anchor` parameter.

## Discussion

The constraint causes the current anchor to trail the object in the `anchor` parameter. For example, in a left-to-right layout, the current anchor is to the right of `anchor`, but in a right-to-left layout, it’s to the left of `anchor`.

The minimum distance between the two anchors is determined by multiplying the system spacing by the value in the `multiplier` parameter. (The actual distance must be greater than or equal to that value.) The value of the system space is determined from information available from the anchors.

## See Also

### Building system spacing constraints

func constraint(equalToSystemSpacingAfter: NSLayoutXAxisAnchor, multiplier: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines by how much the current anchor trails the specified anchor.

func constraint(lessThanOrEqualToSystemSpacingAfter: NSLayoutXAxisAnchor, multiplier: CGFloat) -> NSLayoutConstraint

Returns a constraint that defines the maximum amount by which the current anchor trails the specified anchor.

Creating self-sizing table view cells

Create table view cells that support Dynamic Type and use system spacing constraints to adjust the spacing surrounding text labels.

