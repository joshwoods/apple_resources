

- UIKit
- UIKeyCommand
-  discoverabilityTitle 

Instance Property

# discoverabilityTitle

An elaborated title that explains the purpose of the key command.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var discoverabilityTitle: String? { get set }
```

## Discussion

The system uses this property to display information about the command. In iOS, the system displays this title in the discoverability heads-up display (HUD). If this property is `nil`, the HUD displays the title property.

In Mac apps built with Mac Catalyst, the system displays the discoverability title as a tooltip.

## See Also

### Getting information about the key command

var title: String

The key command’s title.

var image: UIImage?

The key command’s image.

var input: String?

The string of characters corresponding to the keys that must be pressed to match this key command.

var action: Selector?

The command’s action-method selector.

var modifierFlags: UIKeyModifierFlags

The bit mask of modifier flags that must be pressed to match this key command.

struct UIKeyModifierFlags

Constants that indicate which modifier keys are pressed.

var attributes: UIMenuElement.Attributes

The attributes indicating the style of the key command.

var state: UIMenuElement.State

The state of the key command.

