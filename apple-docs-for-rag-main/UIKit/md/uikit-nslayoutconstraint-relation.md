

- UIKit
- NSLayoutConstraint
-  relation 

Instance Property

# relation

The relation between the two attributes in the constraint.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var relation: NSLayoutConstraint.Relation { get }
```

## See Also

### Accessing constraint data

var firstItem: AnyObject?

The first object participating in the constraint.

var firstAttribute: NSLayoutConstraint.Attribute

The attribute of the first object participating in the constraint.

var secondItem: AnyObject?

The second object participating in the constraint.

var secondAttribute: NSLayoutConstraint.Attribute

The attribute of the second object participating in the constraint.

var multiplier: CGFloat

The multiplier applied to the second attribute participating in the constraint.

var constant: CGFloat

The constant added to the multiplied second attribute participating in the constraint.

var firstAnchor: NSLayoutAnchor&lt;AnyObject>

The first anchor that defines the constraint.

var secondAnchor: NSLayoutAnchor&lt;AnyObject>?

The second anchor that defines the constraint.

