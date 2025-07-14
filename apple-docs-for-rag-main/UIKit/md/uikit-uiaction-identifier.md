

- UIKit
- UIAction
-  identifier 

Instance Property

# identifier

The unique identifier for the action.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var identifier: UIAction.Identifier { get }
```

## See Also

### Getting information about the action

var title: String

The action’s title.

var image: UIImage?

The action’s image.

var discoverabilityTitle: String?

An elaborated title that explains the purpose of the action.

var attributes: UIMenuElement.Attributes

The attributes indicating the style of the action.

var state: UIMenuElement.State

The state of the action.

var sender: Any?

The object responsible for the action handler.

