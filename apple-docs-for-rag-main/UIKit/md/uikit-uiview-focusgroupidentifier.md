

- UIKit
- UIView
-  focusGroupIdentifier 

Instance Property

# focusGroupIdentifier

The identifier of the focus group that this view belongs to.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var focusGroupIdentifier: String? { get set }
```

## Discussion

If this property is `nil`, subviews inherit their superview’s focus group.

## See Also

### Working with focus

var canBecomeFocused: Bool

A Boolean value that indicates whether the view is currently capable of being focused.

class var inheritedAnimationDuration: TimeInterval

Returns the inherited duration of the current animation.

var isFocused: Bool

A Boolean value that indicates whether the item is currently focused.

var focusEffect: UIFocusEffect?

The visual effect to apply when the view becomes focused.

var focusGroupPriority: UIFocusGroupPriority

The importance of the item within a focus group, used by the focus system to determine the group’s primary item.

