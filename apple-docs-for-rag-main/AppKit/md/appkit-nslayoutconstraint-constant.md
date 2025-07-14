

- AppKit
- NSLayoutConstraint
-  constant 

Instance Property

# constant

The constant added to the multiplied second attribute participating in the constraint.

macOS 10.7+

``` source
var constant: CGFloat { get set }
```

## Discussion

Unlike the other properties, the constant can be modified after constraint creation. Setting the constant on an existing constraint performs much better than removing the constraint and adding a new one that’s exactly like the old except that it has a different constant.

## See Also

### Accessing constraint data

var firstItem: AnyObject?

The first object participating in the constraint.

var firstAttribute: NSLayoutConstraint.Attribute

The attribute of the first object participating in the constraint.

var relation: NSLayoutConstraint.Relation

The relation between the two attributes in the constraint.

var secondItem: AnyObject?

The second object participating in the constraint.

var secondAttribute: NSLayoutConstraint.Attribute

The attribute of the second object participating in the constraint.

var multiplier: CGFloat

The multiplier applied to the second attribute participating in the constraint.

var firstAnchor: NSLayoutAnchor&lt;AnyObject>

The first anchor that defines the constraint.

var secondAnchor: NSLayoutAnchor&lt;AnyObject>?

The second anchor that defines the constraint.

