

- UIKit
- UICommand
-  attributes 

Instance Property

# attributes

The attributes indicating the style of the command.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var attributes: UIMenuElement.Attributes { get set }
```

## See Also

### Getting information about the command

var title: String

The command’s title.

var image: UIImage?

The command’s image.

var action: Selector

The selector identifying the action method called after the user selects the command.

var discoverabilityTitle: String?

An elaborated title that explains the purpose of the command.

var state: UIMenuElement.State

The state of the command.

