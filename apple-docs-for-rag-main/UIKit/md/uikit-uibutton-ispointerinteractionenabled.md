

- UIKit
- UIButton
-  isPointerInteractionEnabled 

Instance Property

# isPointerInteractionEnabled

A Boolean that enables pointer interaction.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
var isPointerInteractionEnabled: Bool { get set }
```

## Discussion

The default value of this property is false.

## See Also

### Supporting pointer interactions

var isHovered: Bool

A Boolean value that indicates whether a pointer effect is active.

var pointerStyleProvider: UIButton.PointerStyleProvider?

A closure that returns the pointer style to use when the pointer hovers over the button.

typealias PointerStyleProvider

A type alias defining a closure that returns a pointer style to apply to a button.

typealias UIButtonPointerStyleProvider

A type alias defining a block that returns a pointer style to apply to a button.

