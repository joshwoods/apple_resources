

- UIKit
- UIFocusItem
-  canBecomeFocused 

Instance Property

# canBecomeFocused

A Boolean value that indicates whether the item can become focused.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var canBecomeFocused: Bool { get }
```

**Required**

## Mentioned in 

About focus interactions for Apple TV

## Discussion

When the value of this property is false, the item is not focusable, even if it is visible in the user interface. For example, a subclass of UIControl returns false when it is not enabled.

Returning true in this property means that the item is capable of being focused; it does not guarantee that the item is always focusable. Focusability is ultimately determined by the system. For example, if an item is visually obscured or offscreen, it may not be focusable. In addition, objects that conform to this protocol may have their own unique limitations. For example, a UIView object is not focusable when user interaction is disabled, or when the view’s alpha value is equal to `0`.

## See Also

### Determining focusability

var isFocused: Bool

A Boolean value that indicates whether the item is currently focused.

