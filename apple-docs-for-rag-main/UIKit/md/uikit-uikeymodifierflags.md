

- UIKit
-  UIKeyModifierFlags 

Structure

# UIKeyModifierFlags

Constants that indicate which modifier keys are pressed.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
struct UIKeyModifierFlags
```

## Topics

### Modifier flags

static var alphaShift: UIKeyModifierFlags

A modifier flag that indicates the user pressed the Caps Lock key.

static var shift: UIKeyModifierFlags

A modifier flag that indicates the user pressed the Shift key.

static var control: UIKeyModifierFlags

A modifier flag that indicates the user pressed the Control key.

static var alternate: UIKeyModifierFlags

A modifier flag that indicates the user pressed the Option key.

static var command: UIKeyModifierFlags

A modifier flag that indicates the user pressed the Command key.

static var numericPad: UIKeyModifierFlags

A modifier flag that indicates the user pressed a key located on the numeric keypad.

### Initializers

init(rawValue: Int)

Creates a modifier-flags structure from data in an unarchiver.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

var discoverabilityTitle: String?

An elaborated title that explains the purpose of the key command.

var attributes: UIMenuElement.Attributes

The attributes indicating the style of the key command.

var state: UIMenuElement.State

The state of the key command.

