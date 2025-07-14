

- UIKit
- UICommand
-  image 

Instance Property

# image

The command’s image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var image: UIImage? { get set }
```

## Discussion

Only the context menu system supports the display of an image, and only when the app is running in iOS.

## See Also

### Getting information about the command

var title: String

The command’s title.

var action: Selector

The selector identifying the action method called after the user selects the command.

var discoverabilityTitle: String?

An elaborated title that explains the purpose of the command.

var attributes: UIMenuElement.Attributes

The attributes indicating the style of the command.

var state: UIMenuElement.State

The state of the command.

