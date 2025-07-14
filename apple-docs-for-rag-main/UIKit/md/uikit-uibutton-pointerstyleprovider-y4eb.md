

- UIKit
- UIButton
-  pointerStyleProvider 

Instance Property

# pointerStyleProvider

A closure that returns the pointer style to use when the pointer hovers over the button.

iOS 13.4+iPadOS 13.4+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
var pointerStyleProvider: UIButton.PointerStyleProvider? { get set }
```

## Discussion

To change the appearance of the pointer when it hovers over the button, create a UIButton.PointerStyleProvider closure that returns a UIPointerStyle describing the pointer shape and content effect. Then assign the closure to pointerStyleProvider. For example, the following code listing creates a pointer style that applies a lift effect to the button when the pointer hovers over it.

```
threadColorButton.pointerStyleProvider = { button, proposedEffect, proposedShape -> UIPointerStyle? in
    let cornerRadius: CGFloat = 4
    let parameters = UIPreviewParameters()
    let shapePath = UIBezierPath(roundedRect: button.bounds, cornerRadius: cornerRadius)
    parameters.shadowPath = shapePath
    let preview = UITargetedPreview(view: proposedEffect.preview.view, parameters: parameters, target: proposedEffect.preview.target)

    let rect = button.convert(button.bounds, to: preview.target.container)
    return UIPointerStyle(effect: .lift(preview), shape: .roundedRect(rect, radius: cornerRadius))
}
```

For more information, see Enhancing your iPad app with pointer interactions.

## See Also

### Supporting pointer interactions

var isPointerInteractionEnabled: Bool

A Boolean that enables pointer interaction.

var isHovered: Bool

A Boolean value that indicates whether a pointer effect is active.

typealias PointerStyleProvider

A type alias defining a closure that returns a pointer style to apply to a button.

typealias UIButtonPointerStyleProvider

A type alias defining a block that returns a pointer style to apply to a button.

