

- UIKit
- UIAction
-  image 

Instance Property

# image

The action’s image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var image: UIImage? { get set }
```

## Discussion

The image appears next to the action’s title. Only the context menu system supports the display of an image, and only when the app is running in iOS.

## See Also

### Getting information about the action

var title: String

The action’s title.

var identifier: UIAction.Identifier

The unique identifier for the action.

var discoverabilityTitle: String?

An elaborated title that explains the purpose of the action.

var attributes: UIMenuElement.Attributes

The attributes indicating the style of the action.

var state: UIMenuElement.State

The state of the action.

var sender: Any?

The object responsible for the action handler.

