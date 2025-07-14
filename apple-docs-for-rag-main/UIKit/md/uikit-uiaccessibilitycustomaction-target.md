

- UIKit
- UIAccessibilityCustomAction
-  target 

Instance Property

# target

The object that performs the action.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var target: AnyObject? { get set }
```

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

var selector: Selector

The method that performs the action.

typealias Handler

A closure type that defines a handler to perform for an action.

