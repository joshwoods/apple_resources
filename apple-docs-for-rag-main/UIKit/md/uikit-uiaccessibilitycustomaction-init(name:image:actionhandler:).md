

- UIKit
- UIAccessibilityCustomAction
-  init(name:image:actionHandler:) 

Initializer

# init(name:image:actionHandler:)

Creates a custom action object with the specified name, image, and action handler.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
init(
    name: String,
    image: UIImage?,
    actionHandler: @escaping UIAccessibilityCustomAction.Handler
)
```

## See Also

### Creating a custom action

init(name: String, actionHandler: UIAccessibilityCustomAction.Handler)

Creates a custom action object with the specified name and action handler.

init(name: String, target: Any?, selector: Selector)

Creates a custom action object with the specified name, target, and selector.

init(name: String, image: UIImage?, target: Any?, selector: Selector)

Creates a custom action object with the specified name, image, target, and selector.

init(attributedName: NSAttributedString, actionHandler: UIAccessibilityCustomAction.Handler)

Creates a custom action object with the specified attributed name and action handler.

init(attributedName: NSAttributedString, target: Any?, selector: Selector)

Creates a custom action object with the specified attributed name, target, and selector.

init(attributedName: NSAttributedString, image: UIImage?, actionHandler: UIAccessibilityCustomAction.Handler)

Creates a custom action object with the specified attributed name, image, and action handler.

init(attributedName: NSAttributedString, image: UIImage?, target: Any?, selector: Selector)

Creates a custom action object with the specified attributed name, image, target, and selector.

