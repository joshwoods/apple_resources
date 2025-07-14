

- UIKit
- UIAction
-  sender 

Instance Property

# sender

The object responsible for the action handler.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var sender: Any? { get }
```

## See Also

### Getting information about the action

var title: String

The action’s title.

var image: UIImage?

The action’s image.

var identifier: UIAction.Identifier

The unique identifier for the action.

var discoverabilityTitle: String?

An elaborated title that explains the purpose of the action.

var attributes: UIMenuElement.Attributes

The attributes indicating the style of the action.

var state: UIMenuElement.State

The state of the action.

