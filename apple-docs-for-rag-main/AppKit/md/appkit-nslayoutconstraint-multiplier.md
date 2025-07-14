

- AppKit
- NSLayoutConstraint
-  multiplier 

Instance Property

# multiplier

The multiplier applied to the second attribute participating in the constraint.

macOS 10.7+

``` source
var multiplier: CGFloat { get }
```

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

var constant: CGFloat

The constant added to the multiplied second attribute participating in the constraint.

var firstAnchor: NSLayoutAnchor&lt;AnyObject>

The first anchor that defines the constraint.

var secondAnchor: NSLayoutAnchor&lt;AnyObject>?

The second anchor that defines the constraint.

