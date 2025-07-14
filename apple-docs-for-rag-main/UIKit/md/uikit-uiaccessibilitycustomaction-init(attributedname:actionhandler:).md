

- UIKit
- UIAccessibilityCustomAction
-  init(attributedName:actionHandler:) 

Initializer

# init(attributedName:actionHandler:)

Creates a custom action object with the specified attributed name and action handler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init(
    attributedName: NSAttributedString,
    actionHandler: @escaping UIAccessibilityCustomAction.Handler
)
```

## See Also

### Creating a custom action

init(name: String, actionHandler: UIAccessibilityCustomAction.Handler)

Creates a custom action object with the specified name and action handler.

init(name: String, target: Any?, selector: Selector)

Creates a custom action object with the specified name, target, and selector.

init(name: String, image: UIImage?, actionHandler: UIAccessibilityCustomAction.Handler)

Creates a custom action object with the specified name, image, and action handler.

init(name: String, image: UIImage?, target: Any?, selector: Selector)

Creates a custom action object with the specified name, image, target, and selector.

init(attributedName: NSAttributedString, target: Any?, selector: Selector)

Creates a custom action object with the specified attributed name, target, and selector.

init(attributedName: NSAttributedString, image: UIImage?, actionHandler: UIAccessibilityCustomAction.Handler)

Creates a custom action object with the specified attributed name, image, and action handler.

init(attributedName: NSAttributedString, image: UIImage?, target: Any?, selector: Selector)

Creates a custom action object with the specified attributed name, image, target, and selector.

