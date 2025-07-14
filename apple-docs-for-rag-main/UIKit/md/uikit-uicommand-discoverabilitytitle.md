

- UIKit
- UICommand
-  discoverabilityTitle 

Instance Property

# discoverabilityTitle

An elaborated title that explains the purpose of the command.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var discoverabilityTitle: String? { get set }
```

## Discussion

The system uses this property to display information about the command. In iOS, the system displays this title in the discoverability heads-up display (HUD). If this property is `nil`, the HUD displays the title property.

In Mac apps built with Mac Catalyst, the system displays the discoverability title as a tooltip.

## See Also

### Getting information about the command

var title: String

The command’s title.

var image: UIImage?

The command’s image.

var action: Selector

The selector identifying the action method called after the user selects the command.

var attributes: UIMenuElement.Attributes

The attributes indicating the style of the command.

var state: UIMenuElement.State

The state of the command.

