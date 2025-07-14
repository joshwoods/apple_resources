

- UIKit
- UIKeyCommand
-  state 

Instance Property

# state

The state of the key command.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var state: UIMenuElement.State { get set }
```

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

var discoverabilityTitle: String?

An elaborated title that explains the purpose of the key command.

var attributes: UIMenuElement.Attributes

The attributes indicating the style of the key command.

