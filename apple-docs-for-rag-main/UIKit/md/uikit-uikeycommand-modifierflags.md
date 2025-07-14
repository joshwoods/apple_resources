

- UIKit
- UIKeyCommand
-  modifierFlags 

Instance Property

# modifierFlags

The bit mask of modifier flags that must be pressed to match this key command.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var modifierFlags: UIKeyModifierFlags { get }
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

struct UIKeyModifierFlags

Constants that indicate which modifier keys are pressed.

var discoverabilityTitle: String?

An elaborated title that explains the purpose of the key command.

var attributes: UIMenuElement.Attributes

The attributes indicating the style of the key command.

var state: UIMenuElement.State

The state of the key command.

