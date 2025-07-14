

- UIKit
- UIView
-  canBecomeFocused 

Instance Property

# canBecomeFocused

A Boolean value that indicates whether the view is currently capable of being focused.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var canBecomeFocused: Bool { get }
```

## Discussion

The value of this property is true if the view can become focused; false otherwise.

By default, the value of this property is false. This property informs the focus engine if a view is capable of being focused. Sometimes even if a view returns true, a view may not be focusable for the following reasons:

- The view is hidden.

- The view has alpha set to 0.

- The view has `userInteractionEnabled` set to false.

- The view is not currently in the view hierarchy.

## See Also

### Working with focus

class var inheritedAnimationDuration: TimeInterval

Returns the inherited duration of the current animation.

var isFocused: Bool

A Boolean value that indicates whether the item is currently focused.

var focusGroupIdentifier: String?

The identifier of the focus group that this view belongs to.

var focusEffect: UIFocusEffect?

The visual effect to apply when the view becomes focused.

var focusGroupPriority: UIFocusGroupPriority

The importance of the item within a focus group, used by the focus system to determine the group’s primary item.

