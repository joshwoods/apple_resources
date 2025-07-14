

- UIKit
- UIView
-  isFocused 

Instance Property

# isFocused

A Boolean value that indicates whether the item is currently focused.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var isFocused: Bool { get }
```

## Discussion

This is a convenience property that checks whether the item is equal to the value in the UIScreen class’s focusedView property.

## See Also

### Working with focus

var canBecomeFocused: Bool

A Boolean value that indicates whether the view is currently capable of being focused.

class var inheritedAnimationDuration: TimeInterval

Returns the inherited duration of the current animation.

var focusGroupIdentifier: String?

The identifier of the focus group that this view belongs to.

var focusEffect: UIFocusEffect?

The visual effect to apply when the view becomes focused.

var focusGroupPriority: UIFocusGroupPriority

The importance of the item within a focus group, used by the focus system to determine the group’s primary item.

