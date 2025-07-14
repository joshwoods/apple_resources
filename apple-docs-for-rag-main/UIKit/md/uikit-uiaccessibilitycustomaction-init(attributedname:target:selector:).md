

- UIKit
- UIAccessibilityCustomAction
-  init(attributedName:target:selector:) 

Initializer

# init(attributedName:target:selector:)

Creates a custom action object with the specified attributed name, target, and selector.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
init(
    attributedName: NSAttributedString,
    target: Any?,
    selector: Selector
)
```

## Parameters 

`attributedName`  

The localized name of the action. Provide a short and descriptive name for the action.

`target`  

The object that performs the action.

`selector`  

The selector of target to call when you want to perform the action. The method signature must take one of the following forms:

```
- (BOOL)myPerformActionMethod
- (BOOL)myPerformActionMethod:(UIAccessibilityCustomAction *)action
```

## Return Value

An initialized custom action object.

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

init(attributedName: NSAttributedString, actionHandler: UIAccessibilityCustomAction.Handler)

Creates a custom action object with the specified attributed name and action handler.

init(attributedName: NSAttributedString, image: UIImage?, actionHandler: UIAccessibilityCustomAction.Handler)

Creates a custom action object with the specified attributed name, image, and action handler.

init(attributedName: NSAttributedString, image: UIImage?, target: Any?, selector: Selector)

Creates a custom action object with the specified attributed name, image, target, and selector.

