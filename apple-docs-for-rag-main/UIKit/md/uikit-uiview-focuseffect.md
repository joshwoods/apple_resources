

- UIKit
- UIView
-  focusEffect 

Instance Property

# focusEffect

The visual effect to apply when the view becomes focused.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var focusEffect: UIFocusEffect? { get set }
```

## Discussion

If this property is `nil`, the system doesn’t apply an effect when the view becomes focused.

## See Also

### Working with focus

var canBecomeFocused: Bool

A Boolean value that indicates whether the view is currently capable of being focused.

class var inheritedAnimationDuration: TimeInterval

Returns the inherited duration of the current animation.

var isFocused: Bool

A Boolean value that indicates whether the item is currently focused.

var focusGroupIdentifier: String?

The identifier of the focus group that this view belongs to.

var focusGroupPriority: UIFocusGroupPriority

The importance of the item within a focus group, used by the focus system to determine the group’s primary item.

