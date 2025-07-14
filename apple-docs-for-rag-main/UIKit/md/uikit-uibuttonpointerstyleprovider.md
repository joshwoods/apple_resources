

- UIKit
-  UIButtonPointerStyleProvider 

Type Alias

# UIButtonPointerStyleProvider

A type alias defining a block that returns a pointer style to apply to a button.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
typealias UIButtonPointerStyleProvider = (UIButton, __UIPointerEffect, __UIPointerShape) -> UIPointerStyle?
```

## Parameters 

`button`  

The button requesting the pointer style.

`proposedEffect`  

The content effect that the system suggests.

`proposedShape`  

The shape of the pointer that the system suggests.

## Return Value

The pointer style to apply to the button when the pointer hovers over it. Return `nil` when you don’t want to apply a pointer style to the button.

## Discussion

To change the appearance of the pointer when it hovers over the button, create a pointer style provider block and assign it to the button’s pointerStyleProvider property.

## See Also

### Supporting pointer interactions

var isPointerInteractionEnabled: Bool

A Boolean that enables pointer interaction.

var isHovered: Bool

A Boolean value that indicates whether a pointer effect is active.

var pointerStyleProvider: UIButton.PointerStyleProvider?

A closure that returns the pointer style to use when the pointer hovers over the button.

typealias PointerStyleProvider

A type alias defining a closure that returns a pointer style to apply to a button.

