

- UIKit
- NSLayoutConstraint
-  firstAnchor 

Instance Property

# firstAnchor

The first anchor that defines the constraint.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var firstAnchor: NSLayoutAnchor { get }
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

var multiplier: CGFloat

The multiplier applied to the second attribute participating in the constraint.

var constant: CGFloat

The constant added to the multiplied second attribute participating in the constraint.

var secondAnchor: NSLayoutAnchor&lt;AnyObject>?

The second anchor that defines the constraint.

