

- UIKit
- UIAccessibilityCustomAction
-  selector 

Instance Property

# selector

The method that performs the action.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var selector: Selector { get set }
```

## Discussion

The signature of the selector must take one of the following forms:

```
- (BOOL)myPerformActionMethod
- (BOOL)myPerformActionMethod:(UIAccessibilityCustomAction *)action
```

When the user selects a custom action, the assistive technology calls the specified method of the object in the target property. Use your method to perform the indicated action.

## See Also

### Accessing the action parameters

var name: String

The localized name of the action.

var attributedName: NSAttributedString

The localized name of the action as an attributed string.

var image: UIImage?

An image that represents the action in assistive apps.

var actionHandler: UIAccessibilityCustomAction.Handler?

A handler to perform for the action.

var target: AnyObject?

The object that performs the action.

typealias Handler

A closure type that defines a handler to perform for an action.

