

- UIKit
- UIButton
-  isHovered 

Instance Property

# isHovered

A Boolean value that indicates whether a pointer effect is active.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var isHovered: Bool { get }
```

## Discussion

If you enable pointer interaction by setting isPointerInteractionEnabled, this property indicates the button has an active pointer effect.

## See Also

### Related Documentation

Pointer interactions

Support pointer interactions in your custom controls and views.

### Supporting pointer interactions

var isPointerInteractionEnabled: Bool

A Boolean that enables pointer interaction.

var pointerStyleProvider: UIButton.PointerStyleProvider?

A closure that returns the pointer style to use when the pointer hovers over the button.

typealias PointerStyleProvider

A type alias defining a closure that returns a pointer style to apply to a button.

typealias UIButtonPointerStyleProvider

A type alias defining a block that returns a pointer style to apply to a button.

