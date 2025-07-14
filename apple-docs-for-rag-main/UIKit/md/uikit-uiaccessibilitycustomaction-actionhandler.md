

- UIKit
- UIAccessibilityCustomAction
-  actionHandler 

Instance Property

# actionHandler

A handler to perform for the action.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var actionHandler: UIAccessibilityCustomAction.Handler? { get set }
```

## Discussion

If you set this property, the system chooses this action handler over the target and selector.

## See Also

### Accessing the action parameters

var name: String

The localized name of the action.

var attributedName: NSAttributedString

The localized name of the action as an attributed string.

var image: UIImage?

An image that represents the action in assistive apps.

var target: AnyObject?

The object that performs the action.

var selector: Selector

The method that performs the action.

typealias Handler

A closure type that defines a handler to perform for an action.

