

- UIKit
- UIView
-  inheritedAnimationDuration 

Type Property

# inheritedAnimationDuration

Returns the inherited duration of the current animation.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class var inheritedAnimationDuration: TimeInterval { get }
```

## Return Value

The duration of the current animation.

## Discussion

This method only returns a non-zero value if called within a UIView animation block.

## See Also

### Working with focus

var canBecomeFocused: Bool

A Boolean value that indicates whether the view is currently capable of being focused.

var isFocused: Bool

A Boolean value that indicates whether the item is currently focused.

var focusGroupIdentifier: String?

The identifier of the focus group that this view belongs to.

var focusEffect: UIFocusEffect?

The visual effect to apply when the view becomes focused.

var focusGroupPriority: UIFocusGroupPriority

The importance of the item within a focus group, used by the focus system to determine the group’s primary item.

