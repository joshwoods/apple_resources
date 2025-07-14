

- UIKit
- UIAccessibilityCustomAction
-  attributedName 

Instance Property

# attributedName

The localized name of the action as an attributed string.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var attributedName: NSAttributedString { get set }
```

## See Also

### Accessing the action parameters

var name: String

The localized name of the action.

var image: UIImage?

An image that represents the action in assistive apps.

var actionHandler: UIAccessibilityCustomAction.Handler?

A handler to perform for the action.

var target: AnyObject?

The object that performs the action.

var selector: Selector

The method that performs the action.

typealias Handler

A closure type that defines a handler to perform for an action.

